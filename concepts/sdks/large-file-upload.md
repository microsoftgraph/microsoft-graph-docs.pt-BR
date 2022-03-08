---
title: Upload arquivos grandes usando o Microsoft Graph SDKs
description: Fornece diretrizes para carregar arquivos grandes usando o Microsoft Graph SDKs.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: b3219753303745b6db29adadf1e272e4f85f1b4e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335861"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a>Upload arquivos grandes usando o Microsoft Graph SDKs

Várias entidades na Microsoft Graph suportam carregamentos de arquivo [resumáveis](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) para facilitar o carregamento de arquivos grandes. Em vez de tentar carregar todo o arquivo em uma única solicitação, o arquivo é fatiado em partes menores e uma solicitação é usada para carregar uma única fatia. Para simplificar esse processo, os SDKs do Microsoft Graph implementam uma tarefa de carregamento de arquivo grande que gerencia o carregamento das fatias.

## <a name="upload-large-file-to-onedrive"></a>Upload arquivo grande para OneDrive

## <a name="c"></a>[C#](#tab/csharp)

```csharp
using var fileStream = System.IO.File.OpenRead(filePath);

// Use properties to specify the conflict behavior
// in this case, replace
var uploadProps = new DriveItemUploadableProperties
{
    AdditionalData = new Dictionary<string, object>
    {
        { "@microsoft.graph.conflictBehavior", "replace" }
    }
};

// Create the upload session
// itemPath does not need to be a path to an existing item
var uploadSession = await graphClient.Me.Drive.Root
    .ItemWithPath(itemPath)
    .CreateUploadSession(uploadProps)
    .Request()
    .PostAsync();

// Max slice size must be a multiple of 320 KiB
int maxSliceSize = 320 * 1024;
var fileUploadTask =
    new LargeFileUploadTask<DriveItem>(uploadSession, fileStream, maxSliceSize);

var totalLength = fileStream.Length;
// Create a callback that is invoked after each slice is uploaded
IProgress<long> progress = new Progress<long>(prog => {
    Console.WriteLine($"Uploaded {prog} bytes of {totalLength} bytes");
});

try
{
    // Upload the file
    var uploadResult = await fileUploadTask.UploadAsync(progress);

    Console.WriteLine(uploadResult.UploadSucceeded ?
        $"Upload complete, item ID: {uploadResult.ItemResponse.Id}" :
        "Upload failed");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Error uploading: {ex.ToString()}");
}
```

## <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
const options: OneDriveLargeFileUploadOptions = {
  // Relative path from root to destination folder
  path: itemPath,
  // file is a File object, typically from an <input type="file"/>
  fileName: file.name,
  rangeSize: 1024 * 1024,
  uploadEventHandlers: {
    // Called as each "slice" of the file is uploaded
    progress: (range, e) => {
      console.log(`Uploaded ${range?.minValue} to ${range?.maxValue}`);
    }
  }
};

try {
  // Create FileUpload object
  const fileObject = new FileUpload(file, file.name, file.size);
  // Create a OneDrive upload task
  const uploadTask = await OneDriveLargeFileUploadTask
    .createTaskWithFileObject(client, fileObject, options);

  // Do the upload
  const uploadResult: UploadResult = await uploadTask.upload();

  // The response body will be of the corresponding type of the
  // item being uploaded. For OneDrive, this is a DriveItem
  const driveItem = uploadResult.responseBody as DriveItem;
  console.log(`Uploaded file with ID: ${driveItem.id}`);
  return `Uploaded file with ID: ${driveItem.id}`;
} catch (err) {
  console.log(`Error uploading file: ${JSON.stringify(err)}`);
  return `Error uploading file: ${JSON.stringify(err)}`;
}
```

Como alternativas para usar um `File` objeto para criar um `FileUpload`, você pode usar um `ReadStream` objeto para criar um `StreamUpload`.

```typescript
const fileName = "<FILE_NAME>";
const stats = fs.statSync(`./test/sample_files/${fileName}`);
const totalsize = stats.size;
const readStream = fs.createReadStream(`./test/sample_files/${fileName}`);
const fileObject = new StreamUpload(readStream, fileName, totalsize);
```

Você também pode criar uma implementação personalizada da `FileObject` interface.

```typescript
interface FileObject<T> {
  content: T;
  name: string;
  size: number;
  sliceFile(range: Range): Promise<ArrayBuffer | Blob | Buffer>;
}
```

## <a name="java"></a>[Java](#tab/java)

```java
// Get an input stream for the file
File file = new File(localFilePath);
InputStream fileStream = new FileInputStream(file);
long streamSize = file.length();

// Create a callback used by the upload provider
IProgressCallback callback = new IProgressCallback() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }
};

DriveItemCreateUploadSessionParameterSet uploadParams =
    DriveItemCreateUploadSessionParameterSet.newBuilder()
        .withItem(new DriveItemUploadableProperties()).build();

// Create an upload session
UploadSession uploadSession = graphClient
    .me()
    .drive()
    .root()
    // itemPath like "/Folder/file.txt"
    // does not need to be a path to an existing item
    .itemWithPath(itemPath)
    .createUploadSession(uploadParams)
    .buildRequest()
    .post();

LargeFileUploadTask<DriveItem> largeFileUploadTask =
    new LargeFileUploadTask<DriveItem>
        (uploadSession, graphClient, fileStream, streamSize, DriveItem.class);

// Do the upload
largeFileUploadTask.upload(0, null, callback);
```

---

## <a name="resuming-a-file-upload"></a>Retomar um carregamento de arquivo

Os SDKs Graph Microsoft suportam [a retomada de carregamentos em andamento](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload). Se o aplicativo encontrar uma interrupção de conexão ou um status HTTP 5.x.x durante o carregamento, você poderá retomar o carregamento.

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

```csharp
fileUploadTask.ResumeAsync(progress);
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
const resumedFile: DriveItem = await uploadTask.resume() as DriveItem;
```

### <a name="java"></a>[Java](#tab/java)

> [!NOTE]
> O Java SDK atualmente não dá suporte à retomada de downloads em andamento.

---

## <a name="upload-large-attachment-to-outlook-message"></a>Upload anexo grande para Outlook mensagem

### <a name="c"></a>[C#](#tab/csharp)

```csharp
// Create message
var draftMessage = new Message
{
    Subject = "Large attachment"
};

var savedDraft = await graphClient.Me
    .Messages
    .Request()
    .AddAsync(draftMessage);

using var fileStream = System.IO.File.OpenRead(filePath);
var largeAttachment = new AttachmentItem
{
    AttachmentType = AttachmentType.File,
    Name = "largefile.gif",
    Size = fileStream.Length
};

var uploadSession = await graphClient.Me
    .Messages[savedDraft.Id]
    .Attachments
    .CreateUploadSession(largeAttachment)
    .Request()
    .PostAsync();

// Max slice size must be a multiple of 320 KiB
int maxSliceSize = 320 * 1024;
var fileUploadTask =
    new LargeFileUploadTask<FileAttachment>(uploadSession, fileStream, maxSliceSize);

var totalLength = fileStream.Length;
// Create a callback that is invoked after each slice is uploaded
IProgress<long> progress = new Progress<long>(prog => {
    Console.WriteLine($"Uploaded {prog} bytes of {totalLength} bytes");
});

try
{
    // Upload the file
    var uploadResult = await fileUploadTask.UploadAsync(progress);

    Console.WriteLine(uploadResult.UploadSucceeded ? "Upload complete" : "Upload failed");
}
catch (ServiceException ex)
{
    Console.WriteLine($"Error uploading: {ex.ToString()}");
}
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
// Create an attachment item payload
// file is a File object
const payload = {
  AttachmentItem: {
    attachmentType: 'file',
    name: file.name,
    size: file.size
  }
};

const options: LargeFileUploadTaskOptions = {
  rangeSize: 1024 * 1024,
  // Called as each "slice" of the file is uploaded
  uploadEventHandlers: {
    progress: (range, e) => {
      console.log(`Uploaded ${range?.minValue} to ${range?.maxValue}`);
    }
  }
};

try {
  // Create a draft message
  const draftMsg: Message = await client.api('/me/messages')
    .post({
      subject: 'Large file attachment'
    });

  // Create upload session using draft message's ID
  const uploadSession = await LargeFileUploadTask
    .createUploadSession(client,
      `/me/messages/${draftMsg.id}/attachments/createUploadSession`,
      payload);

  // Create file upload
  // Note you can use StreamUpload or custom implementation of FileObject instead
  const fileObject = new FileUpload(file, file.name, file.size);

  // Create upload task
  const uploadTask = new LargeFileUploadTask(client, fileObject, uploadSession, options);

  // Upload the file
  const uploadResult: UploadResult = await uploadTask.upload();
  return 'Attachment uploaded';
} catch (err) {
  console.log(`Error uploading file: ${JSON.stringify(err)}`);
  return `Error uploading file: ${JSON.stringify(err)}`;
}
```

### <a name="java"></a>[Java](#tab/java)

```java
final String[] scopes = { "Mail.ReadWrite" };
ensureGraphClient(scopes);

final String localFilePath = "largefile.gif";

final Message draftMessage = new Message();
draftMessage.subject = "Large attachment";

final Message savedDraft = graphClient
    .me()
    .messages()
    .buildRequest()
    .post(draftMessage);

File file = new File(localFilePath);
// Get an input stream for the file
InputStream fileStream = new FileInputStream(file);

final AttachmentItem largeAttachment = new AttachmentItem();
largeAttachment.attachmentType = AttachmentType.FILE;
largeAttachment.name = "largefile.gif";
largeAttachment.size = file.length();

final AttachmentCreateUploadSessionParameterSet upParams =
    AttachmentCreateUploadSessionParameterSet.newBuilder()
    .withAttachmentItem(largeAttachment)
    .build();

final UploadSession uploadSession = graphClient
    .me()
    .messages(savedDraft.id)
    .attachments()
    .createUploadSession(upParams)
    .buildRequest()
    .post();

// Create a callback used by the upload provider
IProgressCallback callback = new IProgressCallback() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }
};

LargeFileUploadTask<FileAttachment> uploadTask =
    new LargeFileUploadTask<FileAttachment>
        (uploadSession, graphClient, fileStream, file.length(), FileAttachment.class);

// Do the upload
uploadTask.upload(0, null, callback);
```

---

<!-- markdownlint-enable MD024 -->
