---
title: Obter foto
description: Obtenha profilePhoto especificado ou seus metadados (propriedades profilePhoto ).
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b21e23d3b278c608e11a18137329407d68476049
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510757"
---
# <a name="get-photo"></a><span data-ttu-id="a83c2-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="a83c2-103">Get photo</span></span>

<span data-ttu-id="a83c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a83c2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a83c2-105">Obtenha a [profilePhoto](../resources/profilephoto.md) especificada ou seus metadados (propriedades de profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="a83c2-105">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="a83c2-106">**Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="a83c2-106">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="a83c2-107">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648.</span><span class="sxs-lookup"><span data-stu-id="a83c2-107">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="a83c2-108">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a83c2-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="a83c2-109">Você pode obter os metadados da maior foto disponível ou especificar um tamanho para obter os metadados do tamanho dessa foto.</span><span class="sxs-lookup"><span data-stu-id="a83c2-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="a83c2-110">Se o tamanho solicitado não estiver disponível, você ainda poderá obter um tamanho menor que o usuário carregou e disponibilizou.</span><span class="sxs-lookup"><span data-stu-id="a83c2-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="a83c2-111">Por exemplo, se o usuário carrega uma foto de 504 x 504 pixels, tudo menos o tamanho 648 x 648 da foto estará disponível para download.</span><span class="sxs-lookup"><span data-stu-id="a83c2-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="a83c2-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="a83c2-112">Permissions</span></span>

<span data-ttu-id="a83c2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a83c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a83c2-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a83c2-115">Permission type</span></span>      | <span data-ttu-id="a83c2-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a83c2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a83c2-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a83c2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a83c2-118">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="a83c2-118">For **user** resource:</span></span><br/><span data-ttu-id="a83c2-119">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a83c2-119">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a83c2-120">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="a83c2-120">For **group** resource:</span></span><br /><span data-ttu-id="a83c2-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a83c2-121">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a83c2-122">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="a83c2-122">For **contact** resource:</span></span><br /><span data-ttu-id="a83c2-123">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a83c2-123">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="a83c2-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a83c2-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a83c2-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a83c2-125">Not supported</span></span> |
|<span data-ttu-id="a83c2-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a83c2-126">Application</span></span>                        | <span data-ttu-id="a83c2-127">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="a83c2-127">For **user** resource:</span></span><br/><span data-ttu-id="a83c2-128">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a83c2-128">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a83c2-129">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="a83c2-129">For **group** resource:</span></span><br /><span data-ttu-id="a83c2-130">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a83c2-130">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a83c2-131">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="a83c2-131">For **contact** resource:</span></span><br /><span data-ttu-id="a83c2-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a83c2-132">Contacts.Read, Contacts.ReadWrite</span></span> |

> <span data-ttu-id="a83c2-133">**Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a83c2-133">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="a83c2-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a83c2-134">HTTP request</span></span>

### <a name="get-the-photo"></a><span data-ttu-id="a83c2-135">Obter a foto</span><span class="sxs-lookup"><span data-stu-id="a83c2-135">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="a83c2-136">Obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="a83c2-136">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="a83c2-137">Obter os metadados de um tamanho de página específica.</span><span class="sxs-lookup"><span data-stu-id="a83c2-137">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="a83c2-138">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="a83c2-138">Path parameters</span></span>

|<span data-ttu-id="a83c2-139">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a83c2-139">Parameter</span></span>|<span data-ttu-id="a83c2-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="a83c2-140">Type</span></span>|<span data-ttu-id="a83c2-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a83c2-141">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a83c2-142">tamanho</span><span class="sxs-lookup"><span data-stu-id="a83c2-142">size</span></span>  |<span data-ttu-id="a83c2-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a83c2-143">String</span></span>  | <span data-ttu-id="a83c2-144">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="a83c2-144">A photo size.</span></span> <span data-ttu-id="a83c2-145">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648.</span><span class="sxs-lookup"><span data-stu-id="a83c2-145">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="a83c2-146">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a83c2-146">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="a83c2-147">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a83c2-147">Optional query parameters</span></span>
<span data-ttu-id="a83c2-148">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a83c2-148">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a83c2-149">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a83c2-149">Request headers</span></span>
| <span data-ttu-id="a83c2-150">Nome</span><span class="sxs-lookup"><span data-stu-id="a83c2-150">Name</span></span>       | <span data-ttu-id="a83c2-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="a83c2-151">Type</span></span> | <span data-ttu-id="a83c2-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="a83c2-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a83c2-153">Autorização</span><span class="sxs-lookup"><span data-stu-id="a83c2-153">Authorization</span></span>  | <span data-ttu-id="a83c2-154">string</span><span class="sxs-lookup"><span data-stu-id="a83c2-154">string</span></span>  | <span data-ttu-id="a83c2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a83c2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a83c2-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a83c2-157">Request body</span></span>
<span data-ttu-id="a83c2-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a83c2-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a83c2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="a83c2-159">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="a83c2-160">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="a83c2-160">Response for getting the photo</span></span>
<span data-ttu-id="a83c2-p106">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="a83c2-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="a83c2-163">Resposta para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="a83c2-163">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="a83c2-164">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a83c2-164">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="a83c2-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a83c2-165">Examples</span></span>

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="a83c2-166">Exemplo 1: Obter a foto do usuário conectado com o maior tamanho disponível</span><span class="sxs-lookup"><span data-stu-id="a83c2-166">Example 1: Get the photo for the signed-in user in the largest available size</span></span>
##### <a name="request"></a><span data-ttu-id="a83c2-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a83c2-167">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a><span data-ttu-id="a83c2-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a83c2-168">Response</span></span>
<span data-ttu-id="a83c2-169">Contém os dados binários da foto solicitada.</span><span class="sxs-lookup"><span data-stu-id="a83c2-169">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="a83c2-170">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="a83c2-170">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-use"></a><span data-ttu-id="a83c2-171">Exemplo 2: Obtenha foto 48 x 48 para uso conectado</span><span class="sxs-lookup"><span data-stu-id="a83c2-171">Example 2: Get the 48x48 photo for the signed-in use</span></span>
##### <a name="request"></a><span data-ttu-id="a83c2-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a83c2-172">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="a83c2-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="a83c2-173">Response</span></span>
<span data-ttu-id="a83c2-174">Contém os dados binários da foto de 48x48 solicitada.</span><span class="sxs-lookup"><span data-stu-id="a83c2-174">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="a83c2-175">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="a83c2-175">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="a83c2-176">Exemplo 3: Esta solicitação obtém os metadados da foto do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a83c2-176">Example 3: Get the metadata of the user photo of the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="a83c2-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a83c2-177">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a><span data-ttu-id="a83c2-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a83c2-178">Response</span></span>

<span data-ttu-id="a83c2-179">Os dados de resposta a seguir mostram os metadados da foto.</span><span class="sxs-lookup"><span data-stu-id="a83c2-179">The following response data shows the photo metadata.</span></span>

><span data-ttu-id="a83c2-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a83c2-180">**Note:** The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="a83c2-181">Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="a83c2-181">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="a83c2-182">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a83c2-182">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="a83c2-183">Usando os dados binários da foto solicitada</span><span class="sxs-lookup"><span data-stu-id="a83c2-183">Using the binary data of the requested photo</span></span>

<span data-ttu-id="a83c2-184">Ao usar o ponto de extremidade `/photo/$value` para obter os dados binários de uma foto de perfil, você precisa converter os dados em uma cadeia de caracteres da base 64 para adicioná-la como um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="a83c2-184">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="a83c2-185">Veja aqui um exemplo no JavaScript de como criar uma matriz que você pode passar como o valor do parâmetro `Attachments` de uma [Mensagem do Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="a83c2-185">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="a83c2-186">Confira [Amostra de conexão do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) para ver uma implementação desse exemplo.</span><span class="sxs-lookup"><span data-stu-id="a83c2-186">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="a83c2-187">Se quiser exibir a imagem em uma página da Web, crie um objeto de memória usando a imagem e torne esse objeto a fonte de um elemento de imagem.</span><span class="sxs-lookup"><span data-stu-id="a83c2-187">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="a83c2-188">Veja aqui um exemplo dessa operação no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="a83c2-188">Here is an example in JavaScript of this operation.</span></span>

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
