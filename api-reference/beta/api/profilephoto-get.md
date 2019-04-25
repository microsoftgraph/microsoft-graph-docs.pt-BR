---
title: Obter foto
description: Obtenha a profilePhoto específica ou seus metadados (propriedades **profilePhoto**).
localization_priority: Priority
ms.openlocfilehash: 55bdf01515f654eb1622703f9b846de840bc5611
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538551"
---
# <a name="get-photo"></a><span data-ttu-id="70fad-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="70fad-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70fad-104">Obtenha a [profilePhoto](../resources/profilephoto.md) específica ou seus metadados (propriedades **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="70fad-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="70fad-105">Um método de OBTER a foto na primeira tentativa para recuperar a foto específica do Office 365.</span><span class="sxs-lookup"><span data-stu-id="70fad-105">A GET photo method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="70fad-106">Se a foto não estiver disponível no Office 365, a API tenta recuperar a foto do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70fad-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="70fad-107">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648.</span><span class="sxs-lookup"><span data-stu-id="70fad-107">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="70fad-108">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70fad-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="70fad-109">Você pode obter os metadados da maior foto disponível ou especificar um tamanho para obter os metadados do tamanho dessa foto.</span><span class="sxs-lookup"><span data-stu-id="70fad-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="70fad-110">Se o tamanho solicitado não estiver disponível, você ainda poderá obter um tamanho menor que o usuário carregou e disponibilizou.</span><span class="sxs-lookup"><span data-stu-id="70fad-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="70fad-111">Por exemplo, quando o usuário carrega uma foto de 504x504 pixels, todos os tamanhos de foto ficam disponíveis para baixar, exceto o de 648x648.</span><span class="sxs-lookup"><span data-stu-id="70fad-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span>
<span data-ttu-id="70fad-112">Caso o tamanho especificado não esteja disponível na caixa de correio do usuário ou no Azure Active Directory, o tamanho 1x1 será retornado com o restante dos metadados.</span><span class="sxs-lookup"><span data-stu-id="70fad-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size 1x1 is returned with the rest of the  metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="70fad-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="70fad-113">Permissions</span></span>
<span data-ttu-id="70fad-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70fad-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="70fad-116">**Observação:** o método OBTER foto em beta tem suporte para contas corporativas, de estudante ou pessoais do usuário.</span><span class="sxs-lookup"><span data-stu-id="70fad-116">**Note:** The GET photo method in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="70fad-117">O método OBTER foto metadados, no entanto, tem suporte apenas para contas corporativas ou de estudante do usuário, ficando de fora as contas pessoais.</span><span class="sxs-lookup"><span data-stu-id="70fad-117">The GET photo metadata method, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="70fad-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70fad-118">Permission type</span></span>      | <span data-ttu-id="70fad-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70fad-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70fad-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70fad-120">Delegated (work or school account)</span></span> | <span data-ttu-id="70fad-121">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="70fad-121">For **user** resource:</span></span><br/><span data-ttu-id="70fad-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70fad-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="70fad-123">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="70fad-123">For **group** resource:</span></span><br /><span data-ttu-id="70fad-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70fad-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="70fad-125">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="70fad-125">For **contact** resource:</span></span><br /><span data-ttu-id="70fad-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70fad-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="70fad-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70fad-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="70fad-128">**Observação**: não há suporte para a operação de metadados.</span><span class="sxs-lookup"><span data-stu-id="70fad-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="70fad-129">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="70fad-129">For **user** resource:</span></span><br/><span data-ttu-id="70fad-130">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70fad-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="70fad-131">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="70fad-131">For **contact** resource:</span></span><br /><span data-ttu-id="70fad-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70fad-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="70fad-133">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70fad-133">Application</span></span>                        | <span data-ttu-id="70fad-134">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="70fad-134">For **user** resource:</span></span><br/><span data-ttu-id="70fad-135">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70fad-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="70fad-136">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="70fad-136">For **group** resource:</span></span><br /><span data-ttu-id="70fad-137">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70fad-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="70fad-138">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="70fad-138">For **contact** resource:</span></span><br /><span data-ttu-id="70fad-139">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70fad-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="70fad-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70fad-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="70fad-141">Obter a foto</span><span class="sxs-lookup"><span data-stu-id="70fad-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="70fad-142">Obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="70fad-142">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="70fad-143">Obter os metadados de um tamanho de página específica.</span><span class="sxs-lookup"><span data-stu-id="70fad-143">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="70fad-144">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="70fad-144">Path parameters</span></span>

|<span data-ttu-id="70fad-145">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="70fad-145">**Parameter**</span></span>|<span data-ttu-id="70fad-146">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="70fad-146">**Type**</span></span>|<span data-ttu-id="70fad-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70fad-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="70fad-148">size</span><span class="sxs-lookup"><span data-stu-id="70fad-148">size</span></span>  |<span data-ttu-id="70fad-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70fad-149">String</span></span>  | <span data-ttu-id="70fad-150">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="70fad-150">A photo size.</span></span> <span data-ttu-id="70fad-151">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648.</span><span class="sxs-lookup"><span data-stu-id="70fad-151">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="70fad-152">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70fad-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="70fad-153">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70fad-153">Optional query parameters</span></span>
<span data-ttu-id="70fad-154">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70fad-154">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70fad-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70fad-155">Request headers</span></span>
| <span data-ttu-id="70fad-156">Nome</span><span class="sxs-lookup"><span data-stu-id="70fad-156">Name</span></span>       | <span data-ttu-id="70fad-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="70fad-157">Type</span></span> | <span data-ttu-id="70fad-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="70fad-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70fad-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="70fad-159">Authorization</span></span>  | <span data-ttu-id="70fad-160">string</span><span class="sxs-lookup"><span data-stu-id="70fad-160">string</span></span>  | <span data-ttu-id="70fad-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70fad-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70fad-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70fad-163">Request body</span></span>
<span data-ttu-id="70fad-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70fad-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70fad-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="70fad-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="70fad-166">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="70fad-166">Response for getting the photo</span></span>
<span data-ttu-id="70fad-p108">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="70fad-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="70fad-169">Resposta para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="70fad-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="70fad-170">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70fad-170">If successful, this method returns a `200 OK` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70fad-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="70fad-171">Examples</span></span>

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="70fad-172">Exemplo 1: Obtenha a foto do usuário conectado no maior tamanho disponível</span><span class="sxs-lookup"><span data-stu-id="70fad-172">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

##### <a name="request"></a><span data-ttu-id="70fad-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70fad-173">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="70fad-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="70fad-174">Response</span></span>
<span data-ttu-id="70fad-175">Contém os dados binários da foto solicitada.</span><span class="sxs-lookup"><span data-stu-id="70fad-175">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="70fad-176">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="70fad-176">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a><span data-ttu-id="70fad-177">Exemplo 2: Obtenha foto 48 x 48 para usuário conectado</span><span class="sxs-lookup"><span data-stu-id="70fad-177">Example 2: Get the 48x48 photo for the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="70fad-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70fad-178">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="70fad-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="70fad-179">Response</span></span>
<span data-ttu-id="70fad-180">Contém os dados binários da foto de 48x48 solicitada.</span><span class="sxs-lookup"><span data-stu-id="70fad-180">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="70fad-181">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="70fad-181">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="70fad-182">Exemplo 3: Esta solicitação obtém os metadados da foto do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="70fad-182">Example 3: Get the metadata of the user photo of the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="70fad-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70fad-183">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response"></a><span data-ttu-id="70fad-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="70fad-184">Response</span></span>
<span data-ttu-id="70fad-185">Os dados de resposta a seguir mostram os metadados da foto.</span><span class="sxs-lookup"><span data-stu-id="70fad-185">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="70fad-186">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70fad-186">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="70fad-187">Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="70fad-187">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span> 

><span data-ttu-id="70fad-188">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70fad-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="70fad-189">Usando os dados binários da foto solicitada</span><span class="sxs-lookup"><span data-stu-id="70fad-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="70fad-190">Ao usar o ponto de extremidade `/photo/$value` para obter os dados binários de uma foto de perfil, você precisa converter os dados em uma cadeia de caracteres da base 64 para adicioná-la como um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="70fad-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="70fad-191">Veja aqui um exemplo no JavaScript de como criar uma matriz que você pode passar como o valor do parâmetro `Attachments` de uma [Mensagem do Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="70fad-191">The following JavaScript example shows how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="70fad-192">Confira [Amostra de conexão do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) para ver uma implementação desse exemplo.</span><span class="sxs-lookup"><span data-stu-id="70fad-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="70fad-193">Se quiser exibir a imagem em uma página da Web, crie um objeto de memória usando a imagem e torne esse objeto a fonte de um elemento de imagem.</span><span class="sxs-lookup"><span data-stu-id="70fad-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="70fad-194">Veja aqui um exemplo dessa operação no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="70fad-194">Here is an example in JavaScript of this operation.</span></span>

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
