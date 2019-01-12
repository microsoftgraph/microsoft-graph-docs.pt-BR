---
title: Obter o status de um educationSynchronizationProfile
description: Obter o status de um perfil de sincronização de dados específicos escola no inquilino. A resposta indicará que o status da sincronização.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3b235ca243e6ee0f2ebb442d53a7425fa979d778
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965450"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="f92a6-104">Obter o status de um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="f92a6-104">Get the status of an educationSynchronizationProfile</span></span>

> <span data-ttu-id="f92a6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f92a6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f92a6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f92a6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f92a6-107">Obter o status de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.</span><span class="sxs-lookup"><span data-stu-id="f92a6-107">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f92a6-108">A resposta indicará que o status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="f92a6-108">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="f92a6-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="f92a6-109">Permissions</span></span>
<span data-ttu-id="f92a6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f92a6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f92a6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f92a6-112">Permission type</span></span> | <span data-ttu-id="f92a6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f92a6-113">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f92a6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f92a6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f92a6-115">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f92a6-115">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f92a6-116">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f92a6-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f92a6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f92a6-117">Not supported.</span></span>|
|<span data-ttu-id="f92a6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f92a6-118">Application</span></span>| <span data-ttu-id="f92a6-119">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92a6-119">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f92a6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f92a6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="f92a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f92a6-121">Request headers</span></span>
| <span data-ttu-id="f92a6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f92a6-122">Name</span></span>       | <span data-ttu-id="f92a6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f92a6-123">Type</span></span> | <span data-ttu-id="f92a6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f92a6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f92a6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f92a6-125">Authorization</span></span>  | <span data-ttu-id="f92a6-126">string</span><span class="sxs-lookup"><span data-stu-id="f92a6-126">string</span></span>  | <span data-ttu-id="f92a6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f92a6-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f92a6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f92a6-129">Request body</span></span>
<span data-ttu-id="f92a6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f92a6-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f92a6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92a6-131">Response</span></span>
<span data-ttu-id="f92a6-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92a6-132">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f92a6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f92a6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f92a6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f92a6-134">Request</span></span>
<span data-ttu-id="f92a6-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f92a6-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="f92a6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92a6-136">Response</span></span>
<span data-ttu-id="f92a6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f92a6-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f92a6-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f92a6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
