---
title: Obter foto
description: Obtenha o profilePhoto especificado ou seus metadados (**profilePhoto** propriedades).
ms.openlocfilehash: 6374680e37d409a89b61d3e2244b45ccb29869e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041114"
---
# <a name="get-photo"></a><span data-ttu-id="d39c4-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="d39c4-103">Get photo</span></span>

> <span data-ttu-id="d39c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d39c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d39c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d39c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d39c4-106">Obtenha o especificado [profilePhoto](../resources/profilephoto.md) ou seus metadados (**profilePhoto** propriedades).</span><span class="sxs-lookup"><span data-stu-id="d39c4-106">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="d39c4-107">Um GET foto operação primeiro tentar recuperar a foto especificada do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d39c4-107">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="d39c4-108">Se a foto não está disponível no Office 365, a API tenta recuperar a foto do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d39c4-108">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="d39c4-109">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="d39c4-109">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="d39c4-110">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d39c4-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="d39c4-111">Você pode obter os metadados da maior foto disponível ou especificar um tamanho para obter os metadados do tamanho dessa foto.</span><span class="sxs-lookup"><span data-stu-id="d39c4-111">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="d39c4-112">Se o tamanho solicitado não estiver disponível, você ainda poderá obter um tamanho menor que o usuário carregou e disponibilizou.</span><span class="sxs-lookup"><span data-stu-id="d39c4-112">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="d39c4-113">Por exemplo, quando o usuário carrega uma foto de 504x504 pixels, todos os tamanhos de foto ficam disponíveis para baixar, exceto o de 648x648.</span><span class="sxs-lookup"><span data-stu-id="d39c4-113">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="d39c4-114">Caso o tamanho especificado não esteja disponível na caixa de correio do usuário ou no Azure Active Directory, o tamanho “1x1” será retornado com o restante dos metadados.</span><span class="sxs-lookup"><span data-stu-id="d39c4-114">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="d39c4-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="d39c4-115">Permissions</span></span>
<span data-ttu-id="d39c4-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d39c4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="d39c4-118">**Observação:** A operação de foto GET em beta oferece suporte a trabalho, escola ou contas pessoais do usuário.</span><span class="sxs-lookup"><span data-stu-id="d39c4-118">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="d39c4-119">Operação GET foto metadados, entretanto, suporta apenas o usuário comercial ou contas de escola e contas não pessoais.</span><span class="sxs-lookup"><span data-stu-id="d39c4-119">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="d39c4-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d39c4-120">Permission type</span></span>      | <span data-ttu-id="d39c4-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d39c4-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d39c4-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d39c4-122">Delegated (work or school account)</span></span> | <span data-ttu-id="d39c4-123">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-123">For **user** resource:</span></span><br/><span data-ttu-id="d39c4-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d39c4-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d39c4-125">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-125">For **group** resource:</span></span><br /><span data-ttu-id="d39c4-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d39c4-126">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d39c4-127">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-127">For **contact** resource:</span></span><br /><span data-ttu-id="d39c4-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d39c4-128">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="d39c4-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d39c4-129">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="d39c4-130">**Observação**: não há suporte para a operação de metadados.</span><span class="sxs-lookup"><span data-stu-id="d39c4-130">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="d39c4-131">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-131">For **user** resource:</span></span><br/><span data-ttu-id="d39c4-132">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d39c4-132">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="d39c4-133">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-133">For **contact** resource:</span></span><br /><span data-ttu-id="d39c4-134">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d39c4-134">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="d39c4-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d39c4-135">Application</span></span>                        | <span data-ttu-id="d39c4-136">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-136">For **user** resource:</span></span><br/><span data-ttu-id="d39c4-137">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d39c4-137">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d39c4-138">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-138">For **group** resource:</span></span><br /><span data-ttu-id="d39c4-139">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d39c4-139">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d39c4-140">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="d39c4-140">For **contact** resource:</span></span><br /><span data-ttu-id="d39c4-141">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d39c4-141">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d39c4-142">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d39c4-142">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="d39c4-143">Obtenha a foto</span><span class="sxs-lookup"><span data-stu-id="d39c4-143">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="d39c4-144">Obtenha os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="d39c4-144">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="d39c4-145">Obter os metadados para um tamanho específico de foto</span><span class="sxs-lookup"><span data-stu-id="d39c4-145">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="d39c4-146">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d39c4-146">Path parameters</span></span>

|<span data-ttu-id="d39c4-147">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="d39c4-147">**Parameter**</span></span>|<span data-ttu-id="d39c4-148">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="d39c4-148">**Type**</span></span>|<span data-ttu-id="d39c4-149">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d39c4-149">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d39c4-150">size</span><span class="sxs-lookup"><span data-stu-id="d39c4-150">size</span></span>  |<span data-ttu-id="d39c4-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d39c4-151">String</span></span>  | <span data-ttu-id="d39c4-152">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="d39c4-152">A photo size.</span></span> <span data-ttu-id="d39c4-153">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.</span><span class="sxs-lookup"><span data-stu-id="d39c4-153">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="d39c4-154">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d39c4-154">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d39c4-155">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d39c4-155">Optional query parameters</span></span>
<span data-ttu-id="d39c4-156">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d39c4-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d39c4-157">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d39c4-157">Request headers</span></span>
| <span data-ttu-id="d39c4-158">Nome</span><span class="sxs-lookup"><span data-stu-id="d39c4-158">Name</span></span>       | <span data-ttu-id="d39c4-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="d39c4-159">Type</span></span> | <span data-ttu-id="d39c4-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="d39c4-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d39c4-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="d39c4-161">Authorization</span></span>  | <span data-ttu-id="d39c4-162">string</span><span class="sxs-lookup"><span data-stu-id="d39c4-162">string</span></span>  | <span data-ttu-id="d39c4-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d39c4-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d39c4-165">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d39c4-165">Request body</span></span>
<span data-ttu-id="d39c4-166">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d39c4-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d39c4-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d39c4-167">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="d39c4-168">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="d39c4-168">Response for getting the photo</span></span>
<span data-ttu-id="d39c4-p109">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="d39c4-p109">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="d39c4-171">Resposta para obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="d39c4-171">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="d39c4-172">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d39c4-172">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d39c4-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d39c4-173">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d39c4-174">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d39c4-174">Request 1</span></span>
<span data-ttu-id="d39c4-175">Esta solicitação obtém a foto do usuário conectado, com o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="d39c4-175">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="d39c4-176">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d39c4-176">Response 1</span></span>
<span data-ttu-id="d39c4-p110">Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="d39c4-p110">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="d39c4-179">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d39c4-179">Request 2</span></span>
<span data-ttu-id="d39c4-180">Esta solicitação obtém a foto de 48x48 para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d39c4-180">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="d39c4-181">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d39c4-181">Response 2</span></span>
<span data-ttu-id="d39c4-182">Contém os dados binários da foto de 48x48 solicitada.</span><span class="sxs-lookup"><span data-stu-id="d39c4-182">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="d39c4-183">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="d39c4-183">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="d39c4-184">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="d39c4-184">Request 3</span></span>
<span data-ttu-id="d39c4-185">Esta solicitação obtém os metadados da foto do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d39c4-185">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="d39c4-186">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="d39c4-186">Response 3</span></span>
<span data-ttu-id="d39c4-p112">Os dados de resposta a seguir mostram os metadados da foto. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d39c4-p112">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="d39c4-p113">Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d39c4-p113">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="d39c4-191">Usando os dados binários da foto solicitada</span><span class="sxs-lookup"><span data-stu-id="d39c4-191">Using the binary data of the requested photo</span></span>

<span data-ttu-id="d39c4-192">Ao usar o ponto de extremidade `/photo/$value` para obter os dados binários de uma foto de perfil, você precisa converter os dados em uma cadeia de caracteres da base 64 para adicioná-la como um anexo de email.</span><span class="sxs-lookup"><span data-stu-id="d39c4-192">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="d39c4-193">Veja aqui um exemplo no JavaScript de como criar uma matriz que você pode passar como o valor do parâmetro `Attachments` de uma [Mensagem do Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="d39c4-193">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="d39c4-194">Confira [Amostra de conexão do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) para ver uma implementação desse exemplo.</span><span class="sxs-lookup"><span data-stu-id="d39c4-194">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="d39c4-195">Se quiser exibir a imagem em uma página da Web, crie um objeto de memória usando a imagem e torne esse objeto a fonte de um elemento de imagem.</span><span class="sxs-lookup"><span data-stu-id="d39c4-195">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="d39c4-196">Veja aqui um exemplo dessa operação no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d39c4-196">Here is an example in JavaScript of this operation.</span></span>

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
