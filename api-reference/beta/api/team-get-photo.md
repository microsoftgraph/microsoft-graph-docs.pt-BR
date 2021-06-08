---
title: Obter foto da equipe
description: Obter a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: af4e5a95f4af666210be098eb20836bc713d9a8b
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787159"
---
# <a name="get-team-photo"></a><span data-ttu-id="d13bc-103">Obter foto da equipe</span><span class="sxs-lookup"><span data-stu-id="d13bc-103">Get team photo</span></span>

<span data-ttu-id="d13bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d13bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d13bc-105">Obtenha a foto (imagem) de uma equipe ou metadados da foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-105">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="d13bc-106">Em geral, é uma prática recomendada primeiro tentar recuperar os metadados para o tamanho da foto que você deseja obter para garantir que o tamanho esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="d13bc-106">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="d13bc-107">Depois de recuperar os metadados, use o caminho `/$value` para obter os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-107">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="d13bc-108">Este método tenta primeiro recuperar a foto especificada do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d13bc-108">This method first attempts to retrieve the specified photo from Microsoft 365.</span></span> <span data-ttu-id="d13bc-109">Se a foto não estiver disponível no Microsoft 365, ele tentará recuperar a foto do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d13bc-109">If the photo is not available in Microsoft 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="d13bc-110">A seguir, são apresentados os tamanhos suportados de fotos em HD no Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648 pixels.</span><span class="sxs-lookup"><span data-stu-id="d13bc-110">The following are the supported sizes of HD photos in Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="d13bc-111">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d13bc-111">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="d13bc-112">Você pode obter os metadados da maior foto disponível ou, opcionalmente, especificar um tamanho para obter os metadados para esse tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-112">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="d13bc-113">Se o tamanho solicitado não estiver disponível, você poderá obter um tamanho menor.</span><span class="sxs-lookup"><span data-stu-id="d13bc-113">If the size you request is not available, you can still get a smaller size.</span></span> <span data-ttu-id="d13bc-114">Por exemplo, se a maior foto carregada tiver 504x504 pixels, todos os tamanhos, exceto o de 648x648, estarão disponíveis para download.</span><span class="sxs-lookup"><span data-stu-id="d13bc-114">For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="d13bc-115">Se o tamanho especificado não estiver disponível no Microsoft 365 ou no Azure Active Directory, o tamanho 1x1 será retornado com o restante dos metadados.</span><span class="sxs-lookup"><span data-stu-id="d13bc-115">If the specified size is not available in the Microsoft 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="d13bc-116">Há um limite de 4 MB para o tamanho total da solicitação REST.</span><span class="sxs-lookup"><span data-stu-id="d13bc-116">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="d13bc-117">Isso limita o tamanho da foto a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="d13bc-117">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="d13bc-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="d13bc-118">Permissions</span></span>

<span data-ttu-id="d13bc-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d13bc-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d13bc-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d13bc-121">Permission type</span></span>      | <span data-ttu-id="d13bc-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d13bc-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d13bc-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d13bc-123">Delegated (work or school account)</span></span> | <span data-ttu-id="d13bc-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d13bc-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d13bc-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d13bc-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d13bc-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d13bc-126">Not supported.</span></span>    |
|<span data-ttu-id="d13bc-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d13bc-127">Application</span></span> | <span data-ttu-id="d13bc-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d13bc-128">Not supported.</span></span> |

> <span data-ttu-id="d13bc-129">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d13bc-129">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d13bc-p107">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="d13bc-p107">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d13bc-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d13bc-132">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="d13bc-133">Obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="d13bc-133">Get the metadata of the photo</span></span>

<span data-ttu-id="d13bc-134">Este ponto de extremidade retornará os metadados da foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-134">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="d13bc-135">Se nenhum tamanho for especificado, os metadados para o maior tamanho de foto disponível serão retornados.</span><span class="sxs-lookup"><span data-stu-id="d13bc-135">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="d13bc-136">Obter a foto</span><span class="sxs-lookup"><span data-stu-id="d13bc-136">Get the photo</span></span>

<span data-ttu-id="d13bc-137">Este ponto de extremidade recuperará os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-137">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="d13bc-138">Se nenhum tamanho for especificado, o maior tamanho disponível será retornado.</span><span class="sxs-lookup"><span data-stu-id="d13bc-138">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="d13bc-139">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d13bc-139">Path parameters</span></span>

<span data-ttu-id="d13bc-140">Este método suporta um parâmetro de caminho opcional para especificar o tamanho da foto a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="d13bc-140">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="d13bc-141">Você pode especificar qualquer tamanho até o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="d13bc-141">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="d13bc-142">Obtenha os metadados da foto para determinar o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="d13bc-142">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="d13bc-143">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="d13bc-143">**Parameter**</span></span>|<span data-ttu-id="d13bc-144">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="d13bc-144">**Type**</span></span>|<span data-ttu-id="d13bc-145">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d13bc-145">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d13bc-146">size</span><span class="sxs-lookup"><span data-stu-id="d13bc-146">size</span></span>  |<span data-ttu-id="d13bc-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d13bc-147">String</span></span>  | <span data-ttu-id="d13bc-148">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-148">A photo size.</span></span> <span data-ttu-id="d13bc-149">Os tamanhos suportados das fotos em HD do Microsoft 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648.</span><span class="sxs-lookup"><span data-stu-id="d13bc-149">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="d13bc-150">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d13bc-150">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="d13bc-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d13bc-151">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d13bc-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d13bc-152">Request headers</span></span>

| <span data-ttu-id="d13bc-153">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d13bc-153">Header</span></span>        | <span data-ttu-id="d13bc-154">Valor</span><span class="sxs-lookup"><span data-stu-id="d13bc-154">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="d13bc-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="d13bc-155">Authorization</span></span> | <span data-ttu-id="d13bc-p112">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d13bc-p112">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d13bc-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d13bc-158">Request body</span></span>

<span data-ttu-id="d13bc-159">Não forneça um corpo para esta solicitação.</span><span class="sxs-lookup"><span data-stu-id="d13bc-159">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="d13bc-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d13bc-160">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="d13bc-161">Resposta para obter os metadados de uma foto</span><span class="sxs-lookup"><span data-stu-id="d13bc-161">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="d13bc-162">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e metadados sobre a foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-162">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="d13bc-163">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="d13bc-163">Response for getting the photo</span></span>

<span data-ttu-id="d13bc-164">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="d13bc-164">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="d13bc-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d13bc-165">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="d13bc-166">Exemplo 1: obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="d13bc-166">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="d13bc-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d13bc-167">Request</span></span>

<span data-ttu-id="d13bc-168">Aqui está um exemplo da solicitação para obter os metadados da foto da equipe.</span><span class="sxs-lookup"><span data-stu-id="d13bc-168">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="d13bc-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d13bc-169">Response</span></span>

<span data-ttu-id="d13bc-170">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d13bc-170">Here is an example of the response.</span></span>

> <span data-ttu-id="d13bc-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d13bc-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="d13bc-172">Exemplo 2: obter um tamanho específico da foto da equipe</span><span class="sxs-lookup"><span data-stu-id="d13bc-172">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="d13bc-173">Aqui está um exemplo da solicitação para obter a foto da equipe em um tamanho específico.</span><span class="sxs-lookup"><span data-stu-id="d13bc-173">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="d13bc-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d13bc-174">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="d13bc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d13bc-175">Response</span></span>

<span data-ttu-id="d13bc-176">Contém os dados binários da foto de 240x240 solicitada.</span><span class="sxs-lookup"><span data-stu-id="d13bc-176">Contains the binary data of the requested 240x240 photo.</span></span> <span data-ttu-id="d13bc-177">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="d13bc-177">The HTTP response code is 200.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


