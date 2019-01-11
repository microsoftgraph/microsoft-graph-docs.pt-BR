---
title: Obter foto
description: Obtenha a profilePhoto especificada ou seus metadados (propriedades de profilePhoto).
localization_priority: Priority
ms.openlocfilehash: 6b1a3e54b1145cc2fdcf8ed9e587652d4d7061c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833947"
---
# <a name="get-photo"></a><span data-ttu-id="233a0-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="233a0-103">Get photo</span></span>

<span data-ttu-id="233a0-104">Obtenha a [profilePhoto](../resources/profilephoto.md) especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="233a0-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="233a0-105">**Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="233a0-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="233a0-106">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="233a0-106">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="233a0-107">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="233a0-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="233a0-108">Você pode obter os metadados da maior foto disponível ou especificar um tamanho para obter os metadados do tamanho dessa foto.</span><span class="sxs-lookup"><span data-stu-id="233a0-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="233a0-109">Se o tamanho solicitado não estiver disponível, você ainda poderá obter um tamanho menor que o usuário carregou e disponibilizou.</span><span class="sxs-lookup"><span data-stu-id="233a0-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="233a0-110">Por exemplo, quando o usuário carrega uma foto de 504x504 pixels, todos os tamanhos de foto ficam disponíveis para baixar, exceto o de 648x648.</span><span class="sxs-lookup"><span data-stu-id="233a0-110">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="233a0-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="233a0-111">Permissions</span></span>

<span data-ttu-id="233a0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="233a0-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="233a0-114">Permission type</span></span>      | <span data-ttu-id="233a0-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="233a0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233a0-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="233a0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="233a0-117">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="233a0-117">For **user** resource:</span></span><br/><span data-ttu-id="233a0-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233a0-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="233a0-119">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="233a0-119">For **group** resource:</span></span><br /><span data-ttu-id="233a0-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233a0-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="233a0-121">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="233a0-121">For **contact** resource:</span></span><br /><span data-ttu-id="233a0-122">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="233a0-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="233a0-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="233a0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="233a0-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="233a0-124">Not supported</span></span> |
|<span data-ttu-id="233a0-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="233a0-125">Application</span></span>                        | <span data-ttu-id="233a0-126">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="233a0-126">For **user** resource:</span></span><br/><span data-ttu-id="233a0-127">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233a0-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="233a0-128">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="233a0-128">For **group** resource:</span></span><br /><span data-ttu-id="233a0-129">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233a0-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="233a0-130">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="233a0-130">For **contact** resource:</span></span><br /><span data-ttu-id="233a0-131">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="233a0-131">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="233a0-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="233a0-132">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="233a0-133">Obtenha a foto</span><span class="sxs-lookup"><span data-stu-id="233a0-133">Get the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="233a0-134">Obtenha os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="233a0-134">Get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="233a0-135">Obter os metadados para um tamanho específico de foto</span><span class="sxs-lookup"><span data-stu-id="233a0-135">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="233a0-136">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="233a0-136">Path parameters</span></span>

|<span data-ttu-id="233a0-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="233a0-137">Parameter</span></span>|<span data-ttu-id="233a0-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="233a0-138">Type</span></span>|<span data-ttu-id="233a0-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="233a0-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="233a0-140">size</span><span class="sxs-lookup"><span data-stu-id="233a0-140">size</span></span>  |<span data-ttu-id="233a0-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="233a0-141">String</span></span>  | <span data-ttu-id="233a0-142">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="233a0-142">A photo size.</span></span> <span data-ttu-id="233a0-143">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="233a0-143">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="233a0-144">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="233a0-144">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="233a0-145">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="233a0-145">Optional query parameters</span></span>
<span data-ttu-id="233a0-146">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="233a0-146">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="233a0-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="233a0-147">Request headers</span></span>
| <span data-ttu-id="233a0-148">Nome</span><span class="sxs-lookup"><span data-stu-id="233a0-148">Name</span></span>       | <span data-ttu-id="233a0-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="233a0-149">Type</span></span> | <span data-ttu-id="233a0-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="233a0-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="233a0-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="233a0-151">Authorization</span></span>  | <span data-ttu-id="233a0-152">string</span><span class="sxs-lookup"><span data-stu-id="233a0-152">string</span></span>  | <span data-ttu-id="233a0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="233a0-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="233a0-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="233a0-155">Request body</span></span>
<span data-ttu-id="233a0-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="233a0-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="233a0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="233a0-157">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="233a0-158">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="233a0-158">Response for getting the photo</span></span>
<span data-ttu-id="233a0-p106">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="233a0-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="233a0-161">Resposta para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="233a0-161">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="233a0-162">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="233a0-162">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="233a0-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="233a0-163">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="233a0-164">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="233a0-164">Request 1</span></span>
<span data-ttu-id="233a0-165">Esta solicitação obtém a foto do usuário conectado, com o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="233a0-165">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="233a0-166">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="233a0-166">Response 1</span></span>
<span data-ttu-id="233a0-p107">Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="233a0-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="233a0-169">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="233a0-169">Request 2</span></span>
<span data-ttu-id="233a0-170">Esta solicitação obtém a foto de 48x48 para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="233a0-170">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="233a0-171">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="233a0-171">Response 2</span></span>
<span data-ttu-id="233a0-172">Contém os dados binários da foto de 48x48 solicitada.</span><span class="sxs-lookup"><span data-stu-id="233a0-172">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="233a0-173">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="233a0-173">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="233a0-174">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="233a0-174">Request 3</span></span>
<span data-ttu-id="233a0-175">Esta solicitação obtém os metadados da foto do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="233a0-175">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="233a0-176">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="233a0-176">Response 3</span></span>

<span data-ttu-id="233a0-p109">Os dados de resposta a seguir mostram os metadados da foto. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="233a0-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="233a0-p110">Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="233a0-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="233a0-181">Usando os dados binários da foto solicitada</span><span class="sxs-lookup"><span data-stu-id="233a0-181">Using the binary data of the requested photo</span></span>

<span data-ttu-id="233a0-182">Ao usar o ponto de extremidade `/photo/$value` para obter os dados binários de uma foto de perfil, você precisa converter os dados em uma cadeia de caracteres da base 64 para adicioná-la como um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="233a0-182">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="233a0-183">Veja aqui um exemplo no JavaScript de como criar uma matriz que você pode passar como o valor do parâmetro `Attachments` de uma [Mensagem do Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="233a0-183">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="233a0-184">Confira [Amostra de conexão do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) para ver uma implementação desse exemplo.</span><span class="sxs-lookup"><span data-stu-id="233a0-184">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="233a0-185">Se quiser exibir a imagem em uma página da Web, crie um objeto de memória usando a imagem e torne esse objeto a fonte de um elemento de imagem.</span><span class="sxs-lookup"><span data-stu-id="233a0-185">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="233a0-186">Veja aqui um exemplo dessa operação no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="233a0-186">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
