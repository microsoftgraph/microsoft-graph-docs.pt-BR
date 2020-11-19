---
title: Excluir macOSSoftwareUpdateStateSummary
description: Exclui macOSSoftwareUpdateStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b1f0bfe81190ccab3ed4e16fe77a3bd3870424a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219927"
---
# <a name="delete-macossoftwareupdatestatesummary"></a><span data-ttu-id="c3481-103">Excluir macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="c3481-103">Delete macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="c3481-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3481-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3481-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3481-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3481-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3481-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3481-107">Exclui [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c3481-107">Deletes a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3481-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3481-108">Prerequisites</span></span>
<span data-ttu-id="c3481-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3481-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3481-111">Permission type</span></span>|<span data-ttu-id="c3481-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c3481-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3481-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3481-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3481-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3481-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3481-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3481-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3481-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3481-116">Not supported.</span></span>|
|<span data-ttu-id="c3481-117">Application</span><span class="sxs-lookup"><span data-stu-id="c3481-117">Application</span></span>|<span data-ttu-id="c3481-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3481-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3481-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3481-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c3481-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3481-120">Request headers</span></span>
|<span data-ttu-id="c3481-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3481-121">Header</span></span>|<span data-ttu-id="c3481-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c3481-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3481-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3481-123">Authorization</span></span>|<span data-ttu-id="c3481-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3481-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3481-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3481-125">Accept</span></span>|<span data-ttu-id="c3481-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3481-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3481-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3481-127">Request body</span></span>
<span data-ttu-id="c3481-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3481-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3481-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3481-129">Response</span></span>
<span data-ttu-id="c3481-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3481-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c3481-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3481-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3481-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3481-132">Request</span></span>
<span data-ttu-id="c3481-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3481-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="c3481-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3481-134">Response</span></span>
<span data-ttu-id="c3481-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3481-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




