---
title: Obter foto
description: Obtenha a profilePhoto específica ou seus metadados (propriedades **profilePhoto**).
localization_priority: Priority
ms.openlocfilehash: 759c0ff3ac2585f43ea38963e10b001250702c56
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509627"
---
# <a name="get-photo"></a><span data-ttu-id="8357d-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="8357d-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8357d-104">Obtenha a [profilePhoto](../resources/profilephoto.md) específica ou seus metadados (propriedades **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="8357d-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="8357d-105">Uma primeira tentativa da operação OBTER foto em recuperar a foto específica do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8357d-105">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="8357d-106">Se a foto não estiver disponível no Office 365, a API tenta recuperar a foto do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8357d-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="8357d-107">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="8357d-107">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="8357d-108">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8357d-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="8357d-109">Você pode obter os metadados da maior foto disponível ou especificar um tamanho para obter os metadados do tamanho dessa foto.</span><span class="sxs-lookup"><span data-stu-id="8357d-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="8357d-110">Se o tamanho solicitado não estiver disponível, você ainda poderá obter um tamanho menor que o usuário carregou e disponibilizou.</span><span class="sxs-lookup"><span data-stu-id="8357d-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="8357d-111">Por exemplo, quando o usuário carrega uma foto de 504x504 pixels, todos os tamanhos de foto ficam disponíveis para baixar, exceto o de 648x648.</span><span class="sxs-lookup"><span data-stu-id="8357d-111">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="8357d-112">Caso o tamanho especificado não esteja disponível na caixa de correio do usuário ou no Azure Active Directory, o tamanho “1x1” será retornado com o restante dos metadados.</span><span class="sxs-lookup"><span data-stu-id="8357d-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="8357d-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="8357d-113">Permissions</span></span>
<span data-ttu-id="8357d-p104">Uma das permissões a seguir é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8357d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="8357d-116">**Observação:** a operação OBTER foto em beta tem suporte para contas corporativas, de estudante ou pessoais do usuário.</span><span class="sxs-lookup"><span data-stu-id="8357d-116">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="8357d-117">A operação de metadados OBTER foto, no entanto, tem suporte apenas para contas corporativas ou de estudante do usuário, ficando de fora as contas pessoais.</span><span class="sxs-lookup"><span data-stu-id="8357d-117">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="8357d-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8357d-118">Permission type</span></span>      | <span data-ttu-id="8357d-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8357d-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8357d-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8357d-120">Delegated (work or school account)</span></span> | <span data-ttu-id="8357d-121">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="8357d-121">For **user** resource:</span></span><br/><span data-ttu-id="8357d-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8357d-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8357d-123">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="8357d-123">For **group** resource:</span></span><br /><span data-ttu-id="8357d-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8357d-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8357d-125">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="8357d-125">For **contact** resource:</span></span><br /><span data-ttu-id="8357d-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8357d-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="8357d-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8357d-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="8357d-128">**Observação**: não há suporte para a operação de metadados.</span><span class="sxs-lookup"><span data-stu-id="8357d-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="8357d-129">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="8357d-129">For **user** resource:</span></span><br/><span data-ttu-id="8357d-130">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8357d-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="8357d-131">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="8357d-131">For **contact** resource:</span></span><br /><span data-ttu-id="8357d-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8357d-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="8357d-133">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8357d-133">Application</span></span>                        | <span data-ttu-id="8357d-134">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="8357d-134">For **user** resource:</span></span><br/><span data-ttu-id="8357d-135">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8357d-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8357d-136">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="8357d-136">For **group** resource:</span></span><br /><span data-ttu-id="8357d-137">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8357d-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8357d-138">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="8357d-138">For **contact** resource:</span></span><br /><span data-ttu-id="8357d-139">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8357d-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8357d-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8357d-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="8357d-141">Obter a foto</span><span class="sxs-lookup"><span data-stu-id="8357d-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="8357d-142">Obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="8357d-142">Get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="8357d-143">Obter os metadados de um tamanho de página específica.</span><span class="sxs-lookup"><span data-stu-id="8357d-143">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="8357d-144">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="8357d-144">Path parameters</span></span>

|<span data-ttu-id="8357d-145">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="8357d-145">**Parameter**</span></span>|<span data-ttu-id="8357d-146">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="8357d-146">**Type**</span></span>|<span data-ttu-id="8357d-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8357d-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8357d-148">size</span><span class="sxs-lookup"><span data-stu-id="8357d-148">size</span></span>  |<span data-ttu-id="8357d-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8357d-149">String</span></span>  | <span data-ttu-id="8357d-150">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="8357d-150">A photo size.</span></span> <span data-ttu-id="8357d-151">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="8357d-151">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="8357d-152">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8357d-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8357d-153">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8357d-153">Optional query parameters</span></span>
<span data-ttu-id="8357d-154">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8357d-154">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8357d-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8357d-155">Request headers</span></span>
| <span data-ttu-id="8357d-156">Nome</span><span class="sxs-lookup"><span data-stu-id="8357d-156">Name</span></span>       | <span data-ttu-id="8357d-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="8357d-157">Type</span></span> | <span data-ttu-id="8357d-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="8357d-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8357d-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="8357d-159">Authorization</span></span>  | <span data-ttu-id="8357d-160">string</span><span class="sxs-lookup"><span data-stu-id="8357d-160">string</span></span>  | <span data-ttu-id="8357d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8357d-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8357d-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8357d-163">Request body</span></span>
<span data-ttu-id="8357d-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8357d-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8357d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="8357d-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="8357d-166">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="8357d-166">Response for getting the photo</span></span>
<span data-ttu-id="8357d-p108">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="8357d-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="8357d-169">Resposta para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="8357d-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="8357d-170">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8357d-170">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8357d-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8357d-171">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="8357d-172">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="8357d-172">Request 1</span></span>
<span data-ttu-id="8357d-173">Esta solicitação obtém a foto do usuário conectado, com o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="8357d-173">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="8357d-174">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="8357d-174">Response 1</span></span>
<span data-ttu-id="8357d-p109">Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="8357d-p109">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="8357d-177">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="8357d-177">Request 2</span></span>
<span data-ttu-id="8357d-178">Esta solicitação obtém a foto de 48x48 para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8357d-178">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="8357d-179">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="8357d-179">Response 2</span></span>
<span data-ttu-id="8357d-180">Contém os dados binários da foto de 48x48 solicitada.</span><span class="sxs-lookup"><span data-stu-id="8357d-180">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="8357d-181">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="8357d-181">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="8357d-182">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="8357d-182">Request 3</span></span>
<span data-ttu-id="8357d-183">Esta solicitação obtém os metadados da foto do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8357d-183">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="8357d-184">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="8357d-184">Response 3</span></span>
<span data-ttu-id="8357d-p111">Os dados de resposta a seguir mostram os metadados da foto. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8357d-p111">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="8357d-p112">Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8357d-p112">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="8357d-189">Usando os dados binários da foto solicitada</span><span class="sxs-lookup"><span data-stu-id="8357d-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="8357d-190">Ao usar o ponto de extremidade `/photo/$value` para obter os dados binários de uma foto de perfil, você precisa converter os dados em uma cadeia de caracteres da base 64 para adicioná-la como um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="8357d-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="8357d-191">Veja aqui um exemplo no JavaScript de como criar uma matriz que você pode passar como o valor do parâmetro `Attachments` de uma [Mensagem do Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="8357d-191">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="8357d-192">Confira [Amostra de conexão do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) para ver uma implementação desse exemplo.</span><span class="sxs-lookup"><span data-stu-id="8357d-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="8357d-193">Se quiser exibir a imagem em uma página da Web, crie um objeto de memória usando a imagem e torne esse objeto a fonte de um elemento de imagem.</span><span class="sxs-lookup"><span data-stu-id="8357d-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="8357d-194">Veja aqui um exemplo dessa operação no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8357d-194">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/profilephoto-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
