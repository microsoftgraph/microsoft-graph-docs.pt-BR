---
title: Trabalhando com arquivos no Microsoft Graph
description: Você pode usar o Microsoft Graph para criar um aplicativo que se conecta a arquivos entre bibliotecas de documentos do OneDrive, OneDrive for Business e SharePoint.
localization_priority: Priority
ms.prod: sharepoint
author: ''
doc_type: conceptualPageType
ms.openlocfilehash: 043a380890e361b1ad5d920ba4c32de1e89d98ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035907"
---
# <a name="working-with-files-in-microsoft-graph"></a><span data-ttu-id="1c273-103">Trabalhando com arquivos no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c273-103">Working with files in Microsoft Graph</span></span>

<span data-ttu-id="1c273-104">Você pode usar o Microsoft Graph para criar um aplicativo que se conecta a arquivos entre bibliotecas de documentos do OneDrive, OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1c273-104">You can use Microsoft Graph to create an app that connects with files across OneDrive, OneDrive for Business, and SharePoint document libraries.</span></span>
<span data-ttu-id="1c273-105">Com o Microsoft Graph, é possível criar uma variedade de experiências com arquivos armazenados no Office 365, desde simplesmente armazenar documentos de usuários até cenários de compartilhamento de arquivos complexos.</span><span class="sxs-lookup"><span data-stu-id="1c273-105">With Microsoft Graph, you can build a variety of experiences with files stored in Office 365, from simply storing user documents to complex file-sharing scenarios.</span></span>

<span data-ttu-id="1c273-106">O Microsoft Graph expõe dois tipos de recursos para trabalhar com arquivos:</span><span class="sxs-lookup"><span data-stu-id="1c273-106">Microsoft Graph exposes two resource types for working with files:</span></span>

* <span data-ttu-id="1c273-107">[Drive](drive.md) – Representa um contêiner lógico de arquivos, como uma biblioteca de documentos ou o OneDrive de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1c273-107">[Drive](drive.md) - Represents a logical container of files, like a document library or a user's OneDrive.</span></span>
* <span data-ttu-id="1c273-108">[DriveItem](driveitem.md) – Representa um item dentro de uma unidade, como um documento, uma foto, um vídeo ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="1c273-108">[DriveItem](driveitem.md) - Represents an item within a drive, like a document, photo, video, or folder.</span></span>

<span data-ttu-id="1c273-p102">Grande parte da interação com os arquivos ocorre por meio da interação com recursos **DriveItem**. Veja a seguir um exemplo de recurso Driveitem:</span><span class="sxs-lookup"><span data-stu-id="1c273-p102">Most of the interaction with files occurs through interaction with **DriveItem** resources. The following is an example of a DriveItem resource:</span></span>

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

<span data-ttu-id="1c273-111">Recursos **Drive** e **DriveItem** expõem dados de três maneiras diferentes:</span><span class="sxs-lookup"><span data-stu-id="1c273-111">**Drive** and **DriveItem** resources expose data in three different ways:</span></span>

* <span data-ttu-id="1c273-112">_Propriedades_ (como **id** e **name**) expõem valores simples (cadeias de caracteres, números, boolianos).</span><span class="sxs-lookup"><span data-stu-id="1c273-112">_Properties_ (like **id** and **name**) expose simple values (strings, numbers, Booleans).</span></span>
* <span data-ttu-id="1c273-p103">_Facetas_ (como **file** e **photo**) expõem valores complexos. A presença de facetas **file** ou **folder** indica comportamentos e propriedades de um **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="1c273-p103">_Facets_ (like **file** and **photo**) expose complex values. The presence of **file** or **folder** facets indicates behaviors and properties of a **DriveItem**.</span></span>
* <span data-ttu-id="1c273-115">_Referências_ (como **children** e **thumbnails**) apontam para coleções de outros recursos.</span><span class="sxs-lookup"><span data-stu-id="1c273-115">_References_ (like **children** and **thumbnails**) point to collections of other resources.</span></span>

## <a name="commonly-accessed-resources"></a><span data-ttu-id="1c273-116">Recursos comumente acessados</span><span class="sxs-lookup"><span data-stu-id="1c273-116">Commonly accessed resources</span></span>

<span data-ttu-id="1c273-117">A maioria das solicitações de API para interações de arquivo usa um destes recursos base para acessar **Drive** ou **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="1c273-117">Most API requests for file interactions will use one of these base resources to access a **Drive** or **DriveItem**.</span></span>

| <span data-ttu-id="1c273-118">Caminho</span><span class="sxs-lookup"><span data-stu-id="1c273-118">Path</span></span>                               | <span data-ttu-id="1c273-119">Recurso</span><span class="sxs-lookup"><span data-stu-id="1c273-119">Resource</span></span>
|------------------------------------|-----------------------------------------
| `/me/drive`                        | <span data-ttu-id="1c273-120">OneDrive do usuário</span><span class="sxs-lookup"><span data-stu-id="1c273-120">User's OneDrive</span></span>
| `/me/drives`                       | <span data-ttu-id="1c273-121">Enumerar recursos do OneDrive disponíveis para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1c273-121">Enumerate OneDrive resources available to the user.</span></span>
| `/drives/{drive-id}`               | <span data-ttu-id="1c273-122">Acessar uma determinada **Unidade** com base na ID dessa unidade.</span><span class="sxs-lookup"><span data-stu-id="1c273-122">Access a specific **Drive** by the drive's ID.</span></span>
| `/drives/{drive-id}/root/children` | <span data-ttu-id="1c273-123">Enumerar os recursos **DriveItem** na raiz de um determinada **Unidade**.</span><span class="sxs-lookup"><span data-stu-id="1c273-123">Enumerate the **DriveItem** resources in the root of a specific **Drive**.</span></span>
| `/me/drive/items/{item-id}`        | <span data-ttu-id="1c273-124">Acessar um **DriveItem** no OneDrive do usuário com base em sua ID exclusiva.</span><span class="sxs-lookup"><span data-stu-id="1c273-124">Access a **DriveItem** in the user's OneDrive by its unique ID.</span></span>
| `/me/drive/special/{special-id}`   | <span data-ttu-id="1c273-125">Acessar uma pasta especial (nomeada) no OneDrive do usuário com base em seu nome conhecido.</span><span class="sxs-lookup"><span data-stu-id="1c273-125">Access a special (named) folder in the user's OneDrive by its known name.</span></span>
| `/users/{user-id}/drive`           | <span data-ttu-id="1c273-126">Acessar o OneDrive de outro usuário usando a ID exclusiva desse usuário.</span><span class="sxs-lookup"><span data-stu-id="1c273-126">Access another user's OneDrive by using the user's unique ID.</span></span>
| `/groups/{group-id}/drive`         | <span data-ttu-id="1c273-127">Acessar a biblioteca de documentos padrão de um grupo com base na ID exclusiva desse grupo.</span><span class="sxs-lookup"><span data-stu-id="1c273-127">Access the default document library for a group by the group's unique ID.</span></span>
| `/shares/{share-id}`               | <span data-ttu-id="1c273-128">Acessar **DriveItem** com base em sua **sharedId** ou URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="1c273-128">Access a **DriveItem** by its **sharedId** or sharing URL.</span></span>
| `/sites/{site-id}/drive`           | <span data-ttu-id="1c273-129">Acessar o padrão **Unidade** (biblioteca de documentos) para o [site][] do [SharePoint][]</span><span class="sxs-lookup"><span data-stu-id="1c273-129">Access the default **Drive** (document library) for the given [SharePoint][] [site][]</span></span>
| `/sites/{site-id}/drives`          | <span data-ttu-id="1c273-130">Enumerar as **Unidades** (bibliotecas de documentos) do [site][] do [SharePoint][]</span><span class="sxs-lookup"><span data-stu-id="1c273-130">Enumerate the **Drives** (document libraries) under the given [SharePoint][] [site][]</span></span>

<span data-ttu-id="1c273-p104">Além de endereçar **DriveItem** dentro de **Drive** com base na ID exclusiva, seu aplicativo também pode endereçar **DriveItem** com base no caminho relativo de um recurso conhecido. Para endereçar usando um caminho, um caractere de dois pontos (`:`) é usado para escapar o caminho relativo. Essa tabela fornece um exemplo de diferentes maneiras de usar o caractere de dois-pontos para endereçar um item com base no caminho.</span><span class="sxs-lookup"><span data-stu-id="1c273-p104">In addition to addressing a **DriveItem** within a **Drive** by unique ID, your app can also address a **DriveItem** by relative path from a known resource. To address using a path, the colon (`:`) character is used to escape the relative path. This table provides an example of different ways to use the colon character to address an item by path.</span></span>

| <span data-ttu-id="1c273-134">Caminho</span><span class="sxs-lookup"><span data-stu-id="1c273-134">Path</span></span> | <span data-ttu-id="1c273-135">Recurso</span><span class="sxs-lookup"><span data-stu-id="1c273-135">Resource</span></span> |
|---|---|
| `/me/drive/root:/path/to/file` | <span data-ttu-id="1c273-136">Acessar **DriveItem** com base no caminho relativo para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c273-136">Access a **DriveItem** by path relative to the user's OneDrive root folder.</span></span> |
| `/me/drive/items/{item-id}:/path/to/file` | <span data-ttu-id="1c273-137">Acessar **DriveItem** com base no caminho relativo para outro item (um **DriveItem** com uma faceta **folder**).</span><span class="sxs-lookup"><span data-stu-id="1c273-137">Access a **DriveItem** by path relative to another item (a **DriveItem** with a **folder** facet).</span></span> |
| `/me/drive/root:/path/to/folder:/children` | <span data-ttu-id="1c273-138">Listar os filhos de um **DriveItem** com base no caminho relativo para a raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c273-138">List the children of a **DriveItem** by path relative to the root of the user's OneDrive.</span></span> |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | <span data-ttu-id="1c273-139">Listar os filhos de um **DriveItem** com base no caminho relativo para outro item.</span><span class="sxs-lookup"><span data-stu-id="1c273-139">List the children of a **DriveItem** by path relative to another item.</span></span> |

## <a name="drive-resource"></a><span data-ttu-id="1c273-140">Recurso Drive</span><span class="sxs-lookup"><span data-stu-id="1c273-140">Drive resource</span></span>

<span data-ttu-id="1c273-141">O [recurso de Unidade](drive.md) é o objeto de nível superior no OneDrive do usuário ou em uma biblioteca de documentos do [SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="1c273-141">The [Drive resource](drive.md) is the top-level object within a user's OneDrive or a [SharePoint][] document library.</span></span>
<span data-ttu-id="1c273-142">Quase todas as operações de arquivos serão iniciadas com o endereçamento de um recurso Drive específico.</span><span class="sxs-lookup"><span data-stu-id="1c273-142">Nearly all files operations will start by addressing a specific drive resource.</span></span>

<span data-ttu-id="1c273-143">Um recurso Drive pode ser endereçado pela ID exclusiva da unidade ou pela unidade padrão de um [Usuário](user.md), [Grupo](group.md) ou organização.</span><span class="sxs-lookup"><span data-stu-id="1c273-143">A drive resource can be addressed either by the drive's unique ID or by the default drive for a [User](user.md), [Group](group.md), or organization.</span></span> 

## <a name="driveitem-resource"></a><span data-ttu-id="1c273-144">Recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="1c273-144">DriveItem resource</span></span>

<span data-ttu-id="1c273-p106">[DriveItems](driveitem.md) são os objetos dentro do sistema de arquivos da unidade. Eles podem ser acessados por **id** usando a sintaxe `/items/{item-id}` ou por caminho no sistema de arquivos usando a sintaxe `/root:/path/to/item/`.</span><span class="sxs-lookup"><span data-stu-id="1c273-p106">[DriveItems](driveitem.md) are the objects inside a drive's file system. They can be accessed by their **id** by using `/items/{item-id}` syntax, or by their file system path using the `/root:/path/to/item/` syntax.</span></span>

<span data-ttu-id="1c273-147">DriveItems têm _facetas_ que fornecem dados sobre a identidades e as capacidades do item.</span><span class="sxs-lookup"><span data-stu-id="1c273-147">DriveItems have _facets_ that provide data about the item's identity and capabilities.</span></span>

<span data-ttu-id="1c273-148">DriveItems com uma faceta **folder** atuam como contêineres de itens e têm uma referência **children** que aponta para uma coleção de itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="1c273-148">DriveItems with a **folder** facet act as containers of items, and have a **children** reference, which points to a collection of items under the folder.</span></span>

## <a name="shared-folders-and-remote-items"></a><span data-ttu-id="1c273-149">Pastas compartilhadas e itens remotos</span><span class="sxs-lookup"><span data-stu-id="1c273-149">Shared folders and remote items</span></span>

<span data-ttu-id="1c273-p107">Um usuário pessoal do OneDrive pode adicionar um ou mais itens compartilhados de outra unidade a seu próprio OneDrive. Esses itens compartilhados aparecem como **DriveItem** na coleção **children** com uma faceta [remoteItem](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c273-p107">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a **DriveItem** in the **children** collection with a [remoteItem](remoteitem.md) facet.</span></span>

<span data-ttu-id="1c273-152">Para saber mais sobre como trabalhar com pastas compartilhadas e itens remotos, confira [Itens remotos e pastas compartilhadas](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c273-152">For more information about working with shared folders and remote items, see [Remote items and shared folders](remoteitem.md).</span></span>   

## <a name="sharing-and-permissions"></a><span data-ttu-id="1c273-153">Compartilhamento e permissões</span><span class="sxs-lookup"><span data-stu-id="1c273-153">Sharing and permissions</span></span>

<span data-ttu-id="1c273-p108">Uma das ações mais comuns para bibliotecas de documentos do OneDrive e do SharePoint é compartilhar conteúdo com outras pessoas. O Microsoft Graph permite que seu aplicativo crie [links de compartilhamento](../api/driveitem-createlink.md), [adicione permissões e envie convites](../api/driveitem-invite.md) para itens em uma unidade.</span><span class="sxs-lookup"><span data-stu-id="1c273-p108">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create [sharing links](../api/driveitem-createlink.md), [add permissions and send invitations](../api/driveitem-invite.md) to items in a drive.</span></span>

<span data-ttu-id="1c273-156">O Microsoft Graph também fornece uma maneira de seu aplicativo [acessar conteúdo compartilhado](../api/shares-get.md) diretamente de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="1c273-156">Microsoft Graph also provides a way for your app to [access shared content](../api/shares-get.md) directly from a sharing link.</span></span>

[SharePoint]: sharepoint.md
[site]: site.md
