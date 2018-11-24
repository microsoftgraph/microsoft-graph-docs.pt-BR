# <a name="working-with-files-in-microsoft-graph"></a><span data-ttu-id="102b9-101">Trabalhando com arquivos no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="102b9-101">Working with files in Microsoft Graph</span></span>

<span data-ttu-id="102b9-102">Você pode usar o Microsoft Graph para criar um aplicativo que se conecta com arquivos entre OneDrive, o OneDrive for Business e SharePoint bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="102b9-102">You can use Microsoft Graph to create an app that connects with files across OneDrive, OneDrive for Business, and SharePoint document libraries.</span></span>
<span data-ttu-id="102b9-103">Com o Microsoft Graph, você pode construir uma variedade de experiências com arquivos armazenados no Office 365, de simplesmente armazenar documentos do usuário para cenários de compartilhamento de arquivos complexos.</span><span class="sxs-lookup"><span data-stu-id="102b9-103">With Microsoft Graph, you can build a variety of experiences with files stored in Office 365, from simply storing user documents to complex file-sharing scenarios.</span></span>

<span data-ttu-id="102b9-104">O Microsoft Graph expõe dois tipos de recursos para trabalhar com arquivos:</span><span class="sxs-lookup"><span data-stu-id="102b9-104">Microsoft Graph exposes two resource types for working with files:</span></span>

* <span data-ttu-id="102b9-105">[Drive](drive.md) – Representa um contêiner lógico de arquivos, como uma biblioteca de documentos ou o OneDrive de um usuário.</span><span class="sxs-lookup"><span data-stu-id="102b9-105">[Drive](drive.md) - Represents a logical container of files, like a document library or a user's OneDrive.</span></span>
* <span data-ttu-id="102b9-106">[DriveItem](driveitem.md) – Representa um item dentro de uma unidade, como um documento, uma foto, um vídeo ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="102b9-106">[DriveItem](driveitem.md) - Represents an item within a drive, like a document, photo, video, or folder.</span></span>

<span data-ttu-id="102b9-p102">Grande parte da interação com os arquivos ocorre por meio da interação com recursos **DriveItem**. Veja a seguir um exemplo de recurso Driveitem:</span><span class="sxs-lookup"><span data-stu-id="102b9-p102">Most of the interaction with files occurs through interaction with **DriveItem** resources. The following is an example of a DriveItem resource:</span></span>

```json
{
  "@content.downloadUrl":"https://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

<span data-ttu-id="102b9-109">Recursos **Drive** e **DriveItem** expõem dados de três maneiras diferentes:</span><span class="sxs-lookup"><span data-stu-id="102b9-109">**Drive** and **DriveItem** resources expose data in three different ways:</span></span>

* <span data-ttu-id="102b9-110">_Propriedades_ (como **id** e **name**) expõem valores simples (cadeias de caracteres, números, boolianos).</span><span class="sxs-lookup"><span data-stu-id="102b9-110">_Properties_ (like **id** and **name**) expose simple values (strings, numbers, Booleans).</span></span>
* <span data-ttu-id="102b9-p103">_Facetas_ (como **file** e **photo**) expõem valores complexos. A presença de facetas **file** ou **folder** indica comportamentos e propriedades de um **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="102b9-p103">_Facets_ (like **file** and **photo**) expose complex values. The presence of **file** or **folder** facets indicates behaviors and properties of a **DriveItem**.</span></span>
* <span data-ttu-id="102b9-113">_Referências_ (como **children** e **thumbnails**) apontam para coleções de outros recursos.</span><span class="sxs-lookup"><span data-stu-id="102b9-113">_References_ (like **children** and **thumbnails**) point to collections of other resources.</span></span>

## <a name="commonly-accessed-resources"></a><span data-ttu-id="102b9-114">Recursos comumente acessados</span><span class="sxs-lookup"><span data-stu-id="102b9-114">Commonly accessed resources</span></span>

<span data-ttu-id="102b9-115">A maioria das solicitações de API para interações de arquivo usa um destes recursos base para acessar **Drive** ou **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="102b9-115">Most API requests for file interactions will use one of these base resources to access a **Drive** or **DriveItem**.</span></span>

| <span data-ttu-id="102b9-116">Caminho</span><span class="sxs-lookup"><span data-stu-id="102b9-116">Path</span></span>                               | <span data-ttu-id="102b9-117">Recurso</span><span class="sxs-lookup"><span data-stu-id="102b9-117">Resource</span></span>
|------------------------------------|-----------------------------------------
| `/me/drive`                        | <span data-ttu-id="102b9-118">OneDrive do usuário</span><span class="sxs-lookup"><span data-stu-id="102b9-118">User's OneDrive</span></span>
| `/me/drives`                       | <span data-ttu-id="102b9-119">Enumerar recursos do OneDrive disponíveis para o usuário.</span><span class="sxs-lookup"><span data-stu-id="102b9-119">Enumerate OneDrive resources available to the user.</span></span>
| `/drives/{drive-id}`               | <span data-ttu-id="102b9-120">Acessar uma determinada **Unidade** com base na ID dessa unidade.</span><span class="sxs-lookup"><span data-stu-id="102b9-120">Access a specific **Drive** by the drive's ID.</span></span>
| `/drives/{drive-id}/root/children` | <span data-ttu-id="102b9-121">Enumerar os recursos **DriveItem** na raiz de um determinada **Unidade**.</span><span class="sxs-lookup"><span data-stu-id="102b9-121">Enumerate the **DriveItem** resources in the root of a specific **Drive**.</span></span>
| `/me/drive/items/{item-id}`        | <span data-ttu-id="102b9-122">Acessar um **DriveItem** no OneDrive do usuário com base em sua ID exclusiva.</span><span class="sxs-lookup"><span data-stu-id="102b9-122">Access a **DriveItem** in the user's OneDrive by its unique ID.</span></span>
| `/me/drive/special/{special-id}`   | <span data-ttu-id="102b9-123">Acessar uma pasta especial (nomeada) no OneDrive do usuário com base em seu nome conhecido.</span><span class="sxs-lookup"><span data-stu-id="102b9-123">Access a special (named) folder in the user's OneDrive by its known name.</span></span>
| `/users/{user-id}/drive`           | <span data-ttu-id="102b9-124">Acessar o OneDrive de outro usuário usando a ID exclusiva desse usuário.</span><span class="sxs-lookup"><span data-stu-id="102b9-124">Access another user's OneDrive by using the user's unique ID.</span></span>
| `/groups/{group-id}/drive`         | <span data-ttu-id="102b9-125">Acessar a biblioteca de documentos padrão de um grupo com base na ID exclusiva desse grupo.</span><span class="sxs-lookup"><span data-stu-id="102b9-125">Access the default document library for a group by the group's unique ID.</span></span>
| `/shares/{share-id}`               | <span data-ttu-id="102b9-126">Acessar **DriveItem** com base em sua **sharedId** ou URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="102b9-126">Access a **DriveItem** by its **sharedId** or sharing URL.</span></span>
| `/sites/{site-id}/drive`           | <span data-ttu-id="102b9-127">Acessar o padrão de **unidade** (biblioteca de documentos) para [SharePoint][] determinado [site][]</span><span class="sxs-lookup"><span data-stu-id="102b9-127">Access the default **Drive** (document library) for the given [SharePoint][] [site][]</span></span>
| `/sites/{site-id}/drives`          | <span data-ttu-id="102b9-128">Enumerar as **unidades** (bibliotecas de documentos) em [SharePoint][] determinado [site][]</span><span class="sxs-lookup"><span data-stu-id="102b9-128">Enumerate the **Drives** (document libraries) under the given [SharePoint][] [site][]</span></span>

<span data-ttu-id="102b9-p104">Além de endereçar **DriveItem** dentro de **Drive** com base na ID exclusiva, seu aplicativo também pode endereçar **DriveItem** com base no caminho relativo de um recurso conhecido. Para endereçar usando um caminho, um caractere de dois pontos (`:`) é usado para escapar o caminho relativo. Essa tabela fornece um exemplo de diferentes maneiras de usar o caractere de dois-pontos para endereçar um item com base no caminho.</span><span class="sxs-lookup"><span data-stu-id="102b9-p104">In addition to addressing a **DriveItem** within a **Drive** by unique ID, your app can also address a **DriveItem** by relative path from a known resource. To address using a path, the colon (`:`) character is used to escape the relative path. This table provides an example of different ways to use the colon character to address an item by path.</span></span>

| <span data-ttu-id="102b9-132">Caminho</span><span class="sxs-lookup"><span data-stu-id="102b9-132">Path</span></span> | <span data-ttu-id="102b9-133">Recurso</span><span class="sxs-lookup"><span data-stu-id="102b9-133">Resource</span></span> |
|---|---|
| `/me/drive/root:/path/to/file` | <span data-ttu-id="102b9-134">Acessar **DriveItem** com base no caminho relativo para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="102b9-134">Access a **DriveItem** by path relative to the user's OneDrive root folder.</span></span> |
| `/me/drive/items/{item-id}:/path/to/file` | <span data-ttu-id="102b9-135">Acessar **DriveItem** com base no caminho relativo para outro item (um **DriveItem** com uma faceta **folder**).</span><span class="sxs-lookup"><span data-stu-id="102b9-135">Access a **DriveItem** by path relative to another item (a **DriveItem** with a **folder** facet).</span></span> |
| `/me/drive/root:/path/to/folder:/children` | <span data-ttu-id="102b9-136">Listar os filhos de um **DriveItem** com base no caminho relativo para a raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="102b9-136">List the children of a **DriveItem** by path relative to the root of the user's OneDrive.</span></span> |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | <span data-ttu-id="102b9-137">Listar os filhos de um **DriveItem** com base no caminho relativo para outro item.</span><span class="sxs-lookup"><span data-stu-id="102b9-137">List the children of a **DriveItem** by path relative to another item.</span></span> |

## <a name="drive-resource"></a><span data-ttu-id="102b9-138">Recurso Drive</span><span class="sxs-lookup"><span data-stu-id="102b9-138">Drive resource</span></span>

<span data-ttu-id="102b9-139">O [recurso de unidade](drive.md) é o objeto de nível superior dentro de OneDrive um usuário ou uma biblioteca de documentos do [SharePoint][] .</span><span class="sxs-lookup"><span data-stu-id="102b9-139">The [Drive resource](drive.md) is the top-level object within a user's OneDrive or a [SharePoint][] document library.</span></span>
<span data-ttu-id="102b9-140">Quase todas as operações de arquivos serão iniciadas com o endereçamento de um recurso Drive específico.</span><span class="sxs-lookup"><span data-stu-id="102b9-140">Nearly all files operations will start by addressing a specific drive resource.</span></span>

<span data-ttu-id="102b9-141">Um recurso Drive pode ser endereçado pela ID exclusiva da unidade ou pela unidade padrão de um [Usuário](user.md), [Grupo](group.md) ou organização.</span><span class="sxs-lookup"><span data-stu-id="102b9-141">A drive resource can be addressed either by the drive's unique ID or by the default drive for a [User](user.md), [Group](group.md), or organization.</span></span> 

## <a name="driveitem-resource"></a><span data-ttu-id="102b9-142">Recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="102b9-142">DriveItem resource</span></span>

<span data-ttu-id="102b9-p106">[DriveItems](driveitem.md) são os objetos dentro do sistema de arquivos da unidade. Eles podem ser acessados por **id** usando a sintaxe `/items/{item-id}` ou por caminho no sistema de arquivos usando a sintaxe `/root:/path/to/item/`.</span><span class="sxs-lookup"><span data-stu-id="102b9-p106">[DriveItems](driveitem.md) are the objects inside a drive's file system. They can be accessed by their **id** by using `/items/{item-id}` syntax, or by their file system path using the `/root:/path/to/item/` syntax.</span></span>

<span data-ttu-id="102b9-145">DriveItems têm _facetas_ que fornecem dados sobre a identidades e as capacidades do item.</span><span class="sxs-lookup"><span data-stu-id="102b9-145">DriveItems have _facets_ that provide data about the item's identity and capabilities.</span></span>

<span data-ttu-id="102b9-146">DriveItems com uma faceta **folder** atuam como contêineres de itens e têm uma referência **children** que aponta para uma coleção de itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="102b9-146">DriveItems with a **folder** facet act as containers of items, and have a **children** reference, which points to a collection of items under the folder.</span></span>

## <a name="shared-folders-and-remote-items"></a><span data-ttu-id="102b9-147">Pastas compartilhadas e itens remotos</span><span class="sxs-lookup"><span data-stu-id="102b9-147">Shared folders and remote items</span></span>

<span data-ttu-id="102b9-p107">Um usuário pessoal do OneDrive pode adicionar um ou mais itens compartilhados de outra unidade a seu próprio OneDrive. Esses itens compartilhados aparecem como **DriveItem** na coleção **children** com uma faceta [remoteItem](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="102b9-p107">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a **DriveItem** in the **children** collection with a [remoteItem](remoteitem.md) facet.</span></span>

<span data-ttu-id="102b9-150">Para saber mais sobre como trabalhar com pastas compartilhadas e itens remotos, confira [Itens remotos e pastas compartilhadas](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="102b9-150">For more information about working with shared folders and remote items, see [Remote items and shared folders](remoteitem.md).</span></span>   

## <a name="sharing-and-permissions"></a><span data-ttu-id="102b9-151">Compartilhamento e permissões</span><span class="sxs-lookup"><span data-stu-id="102b9-151">Sharing and permissions</span></span>

<span data-ttu-id="102b9-p108">Uma das ações mais comuns para bibliotecas de documentos do OneDrive e do SharePoint é compartilhar conteúdo com outras pessoas. O Microsoft Graph permite que seu aplicativo crie [links de compartilhamento](../api/driveitem_createlink.md), [adicione permissões e envie convites](../api/driveitem_invite.md) para itens em uma unidade.</span><span class="sxs-lookup"><span data-stu-id="102b9-p108">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create [sharing links](../api/driveitem_createlink.md), [add permissions and send invitations](../api/driveitem_invite.md) to items in a drive.</span></span>

<span data-ttu-id="102b9-154">O Microsoft Graph também fornece uma maneira de seu aplicativo [acessar conteúdo compartilhado](../api/shares_get.md) diretamente de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="102b9-154">Microsoft Graph also provides a way for your app to [access shared content](../api/shares_get.md) directly from a sharing link.</span></span>

[SharePoint]: sharepoint.md
[site]: site.md
