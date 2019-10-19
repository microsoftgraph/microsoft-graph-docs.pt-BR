---
title: Obter foto da equipe
description: Obter a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ab94922ed34b01be43a7776f017341a2b47f474d
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2019
ms.locfileid: "37598230"
---
# <a name="get-team-photo"></a><span data-ttu-id="f7b2a-103">Obter foto da equipe</span><span class="sxs-lookup"><span data-stu-id="f7b2a-103">Get team photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b2a-104">Obtenha a foto (imagem) de uma equipe ou metadados da foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-104">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="f7b2a-105">Em geral, é uma prática recomendada primeiro tentar recuperar os metadados para o tamanho da foto que você deseja obter para garantir que o tamanho esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-105">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="f7b2a-106">Depois de recuperar os metadados, use o caminho `/$value` para obter os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-106">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="f7b2a-107">Este método tenta primeiro recuperar a foto especificada do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-107">This method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="f7b2a-108">Se a foto não estiver disponível no Office 365, ele tentará recuperar a foto do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-108">If the photo is not available in Office 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="f7b2a-109">A seguir, são apresentados os tamanhos suportados de fotos em HD no Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648 pixels.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-109">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="f7b2a-110">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="f7b2a-111">Você pode obter os metadados da maior foto disponível ou, opcionalmente, especificar um tamanho para obter os metadados para esse tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-111">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="f7b2a-112">Se o tamanho solicitado não estiver disponível, você poderá obter um tamanho menor.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-112">If the size you request is not available, you can still get a smaller size.</span></span> <span data-ttu-id="f7b2a-113">Por exemplo, se a maior foto carregada tiver 504x504 pixels, todos os tamanhos, exceto o de 648x648, estarão disponíveis para download.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-113">For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="f7b2a-114">Se o tamanho especificado não estiver disponível no Office 365 ou no Azure Active Directory, o tamanho 1x1 será retornado com o restante dos metadados.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-114">If the specified size is not available in the Office 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="f7b2a-115">Há um limite de 4 MB para o tamanho total da solicitação REST.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-115">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="f7b2a-116">Isso limita o tamanho da foto a menos de 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-116">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b2a-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7b2a-117">Permissions</span></span>

<span data-ttu-id="f7b2a-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7b2a-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7b2a-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7b2a-120">Permission type</span></span>      | <span data-ttu-id="f7b2a-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7b2a-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b2a-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7b2a-122">Delegated (work or school account)</span></span> | <span data-ttu-id="f7b2a-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b2a-123">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7b2a-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7b2a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b2a-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-125">Not supported.</span></span>    |
|<span data-ttu-id="f7b2a-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7b2a-126">Application</span></span> | <span data-ttu-id="f7b2a-127">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b2a-127">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b2a-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b2a-128">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="f7b2a-129">Obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="f7b2a-129">Get the metadata of the photo</span></span>

<span data-ttu-id="f7b2a-130">Este ponto de extremidade retornará os metadados da foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-130">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="f7b2a-131">Se nenhum tamanho for especificado, os metadados para o maior tamanho de foto disponível serão retornados.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-131">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo
GET /beta/teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="f7b2a-132">Obter a foto</span><span class="sxs-lookup"><span data-stu-id="f7b2a-132">Get the photo</span></span>

<span data-ttu-id="f7b2a-133">Este ponto de extremidade recuperará os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-133">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="f7b2a-134">Se nenhum tamanho for especificado, o maior tamanho disponível será retornado.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-134">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="f7b2a-135">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="f7b2a-135">Path parameters</span></span>

<span data-ttu-id="f7b2a-136">Este método suporta um parâmetro de caminho opcional para especificar o tamanho da foto a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-136">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="f7b2a-137">Você pode especificar qualquer tamanho até o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-137">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="f7b2a-138">Obtenha os metadados da foto para determinar o maior tamanho disponível.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-138">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="f7b2a-139">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="f7b2a-139">**Parameter**</span></span>|<span data-ttu-id="f7b2a-140">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="f7b2a-140">**Type**</span></span>|<span data-ttu-id="f7b2a-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7b2a-141">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f7b2a-142">size</span><span class="sxs-lookup"><span data-stu-id="f7b2a-142">size</span></span>  |<span data-ttu-id="f7b2a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7b2a-143">String</span></span>  | <span data-ttu-id="f7b2a-144">Um tamanho de foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-144">A photo size.</span></span> <span data-ttu-id="f7b2a-145">Os tamanhos de fotos em HD compatíveis com o Office 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-145">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="f7b2a-146">As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-146">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="f7b2a-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-147">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f7b2a-148">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b2a-148">Request headers</span></span>

| <span data-ttu-id="f7b2a-149">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7b2a-149">Header</span></span>        | <span data-ttu-id="f7b2a-150">Valor</span><span class="sxs-lookup"><span data-stu-id="f7b2a-150">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="f7b2a-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7b2a-151">Authorization</span></span> | <span data-ttu-id="f7b2a-p111">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-p111">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7b2a-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b2a-154">Request body</span></span>

<span data-ttu-id="f7b2a-155">Não forneça um corpo para esta solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-155">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="f7b2a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b2a-156">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="f7b2a-157">Resposta para obter os metadados de uma foto</span><span class="sxs-lookup"><span data-stu-id="f7b2a-157">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="f7b2a-158">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e metadados sobre a foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-158">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="f7b2a-159">Resposta para obter a foto</span><span class="sxs-lookup"><span data-stu-id="f7b2a-159">Response for getting the photo</span></span>

<span data-ttu-id="f7b2a-160">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e os dados binários da foto.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-160">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="f7b2a-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7b2a-161">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="f7b2a-162">Exemplo 1: obter os metadados da foto</span><span class="sxs-lookup"><span data-stu-id="f7b2a-162">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="f7b2a-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b2a-163">Request</span></span>

<span data-ttu-id="f7b2a-164">Aqui está um exemplo da solicitação para obter os metadados da foto da equipe.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-164">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="f7b2a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b2a-165">Response</span></span>

<span data-ttu-id="f7b2a-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-166">Here is an example of the response.</span></span>

> <span data-ttu-id="f7b2a-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

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

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="f7b2a-169">Exemplo 2: obter um tamanho específico da foto da equipe</span><span class="sxs-lookup"><span data-stu-id="f7b2a-169">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="f7b2a-170">Aqui está um exemplo da solicitação para obter a foto da equipe em um tamanho específico.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-170">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="f7b2a-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b2a-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="f7b2a-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b2a-172">Response</span></span>

<span data-ttu-id="f7b2a-173">Contém os dados binários da foto de 240x240 solicitada.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-173">Contains the binary data of the requested 240x240 photo.</span></span> <span data-ttu-id="f7b2a-174">O código de resposta HTTP é 200.</span><span class="sxs-lookup"><span data-stu-id="f7b2a-174">The HTTP response code is 200.</span></span>

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
