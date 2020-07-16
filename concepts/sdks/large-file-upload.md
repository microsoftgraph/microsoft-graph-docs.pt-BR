---
title: Carregar arquivos grandes usando os SDKs do Microsoft Graph
description: Fornece orientações para carregar arquivos grandes usando os SDKs do Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 44465dcc22dcd84c78ee8aa7abfc1f6dc9e36c8a
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44743996"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a><span data-ttu-id="315df-103">Carregar arquivos grandes usando os SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="315df-103">Upload large files using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="315df-104">Várias entidades no Microsoft Graph dão suporte a [carregamentos de arquivos retomáveis](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0) para facilitar o carregamento de arquivos grandes.</span><span class="sxs-lookup"><span data-stu-id="315df-104">A number of entities in Microsoft Graph support [resumable file uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0) to make it easier to upload large files.</span></span> <span data-ttu-id="315df-105">Em vez de tentar carregar todo o arquivo em uma única solicitação, o arquivo é dividido em partes menores e uma solicitação é usada para carregar uma única fatia.</span><span class="sxs-lookup"><span data-stu-id="315df-105">Instead of trying to upload the entire file in a single request, the file is sliced into smaller pieces and a request is used to upload a single slice.</span></span> <span data-ttu-id="315df-106">Para simplificar esse processo, os SDKs do Microsoft Graph implementam uma tarefa de upload de arquivo grande que gerencia o carregamento das fatias.</span><span class="sxs-lookup"><span data-stu-id="315df-106">In order to simplify this process, the Microsoft Graph SDKs implement a large file upload task that manages the uploading of the slices.</span></span>

## <a name="c"></a>[<span data-ttu-id="315df-107">C#</span><span class="sxs-lookup"><span data-stu-id="315df-107">C#</span></span>](#tab/csharp)

```csharp
using (var fileStream = System.IO.File.OpenRead(filePath))
{
    // Use properties to specify the conflict behavior
    // in this case, replace
    var uploadProps = new DriveItemUploadableProperties
    {
        ODataType = null,
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

    // Create a callback that is invoked after each slice is uploaded
    IProgress<long> progress = new Progress<long>(progress => {
        Console.WriteLine($"Uploaded {progress} bytes of {fileStream.Length} bytes");
    });

    try
    {
        // Upload the file
        var uploadResult = await fileUploadTask.UploadAsync(progress);

        if (uploadResult.UploadSucceeded)
        {
            // The ItemResponse object in the result represents the
            // created item.
            Console.WriteLine($"Upload complete, item ID: {uploadResult.ItemResponse.Id}");
        }
        else
        {
            Console.WriteLine("Upload failed");
        }
    }
    catch (ServiceException ex)
    {
        Console.WriteLine($"Error uploading: {ex.ToString()}");
    }
}
```

## <a name="typescript"></a>[<span data-ttu-id="315df-108">TypeScript</span><span class="sxs-lookup"><span data-stu-id="315df-108">TypeScript</span></span>](#tab/typescript)

```typescript
const options: any = {
    // Relative path from root to destination folder
    path: itemPath,
    // file is a File object, typically from an <input type="file"/>
    fileName: file.name,
    rangeSize: 320 * 1024
  }

  try {
    const uploadTask: MicrosoftGraph.OneDriveLargeFileUploadTask =
      await MicrosoftGraph.OneDriveLargeFileUploadTask.create(client, file, options);

    const uploadedFile: DriveItem = await uploadTask.upload();

    console.log(JSON.stringify(`Uploaded file with ID: ${uploadedFile.id}`));
    return `Uploaded file with ID: ${uploadedFile.id}`;
  } catch (err) {
    console.log(`Error uploading file: ${JSON.stringify(err)}`);
    return `Error uploading file: ${JSON.stringify(err)}`;
  }
}
```

## <a name="java"></a>[<span data-ttu-id="315df-109">Java</span><span class="sxs-lookup"><span data-stu-id="315df-109">Java</span></span>](#tab/java)

```java
// Get an input stream for the file
File file = new File(localFilePath);
InputStream fileStream = new FileInputStream(file);
long streamSize = file.length();

// Create a callback used by the upload provider
IProgressCallback<DriveItem> callback = new IProgressCallback<DriveItem>() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }

    @Override
    public void success(final DriveItem result) {
        System.out.println(
            String.format("Uploaded file with ID: %s", result.id)
        );
    }

    public void failure(final ClientException ex) {
        System.out.println(
            String.format("Error uploading file: %s", ex.getMessage())
        );
    }
};

// Create an upload session
UploadSession uploadSession = graphClient
    .me()
    .drive()
    .root()
    // itemPath like "/Folder/file.txt"
    // does not need to be a path to an existing item
    .itemWithPath(itemPath)
    .createUploadSession(new DriveItemUploadableProperties())
    .buildRequest()
    .post();

ChunkedUploadProvider<DriveItem> chunkedUploadProvider =
    new ChunkedUploadProvider<DriveItem>
        (uploadSession, graphClient, fileStream, streamSize, DriveItem.class);

// Config parameter is an array of integers
// customConfig[0] indicates the max slice size
// Max slice size must be a multiple of 320 KiB
int[] customConfig = { 320 * 1024 };

// Do the upload
chunkedUploadProvider.upload(callback, customConfig);
```

---

## <a name="resuming-a-file-upload"></a><span data-ttu-id="315df-110">Retomando um upload de arquivo</span><span class="sxs-lookup"><span data-stu-id="315df-110">Resuming a file upload</span></span>

<span data-ttu-id="315df-111">Os SDKs do Microsoft Graph dão suporte à [continuação dos carregamentos em andamento](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#resuming-an-in-progress-upload).</span><span class="sxs-lookup"><span data-stu-id="315df-111">The Microsoft Graph SDKs support [resuming in-progress uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#resuming-an-in-progress-upload).</span></span> <span data-ttu-id="315df-112">Se o aplicativo encontrar uma interrupção de conexão ou um status HTTP de 5. x. x durante o carregamento, você poderá retomar o upload.</span><span class="sxs-lookup"><span data-stu-id="315df-112">If your application encounters a connection interruption or a 5.x.x HTTP status during upload, you can resume the upload.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="315df-113">C#</span><span class="sxs-lookup"><span data-stu-id="315df-113">C#</span></span>](#tab/csharp)

```csharp
fileUploadTask.ResumeAsync(progress);
```

### <a name="typescript"></a>[<span data-ttu-id="315df-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="315df-114">TypeScript</span></span>](#tab/typescript)

```typescript
const resumedFile: DriveItem = await uploadTask.resume();
```

### <a name="java"></a>[<span data-ttu-id="315df-115">Java</span><span class="sxs-lookup"><span data-stu-id="315df-115">Java</span></span>](#tab/java)

> [!NOTE]
> <span data-ttu-id="315df-116">No momento, o Java SDK não dá suporte à continuação dos downloads em andamento.</span><span class="sxs-lookup"><span data-stu-id="315df-116">The Java SDK does not currently support resuming in-progress downloads.</span></span>

---
<!-- markdownlint-enable MD024 -->
