---
title: Excluir userExperienceAnalyticsMetricHistory
description: Exclui userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fd7c665ea9d390776548f62c2df6b4905812190
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793146"
---
# <a name="delete-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="c0052-103">Excluir userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="c0052-103">Delete userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="c0052-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0052-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0052-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0052-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0052-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0052-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0052-107">Exclui [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span><span class="sxs-lookup"><span data-stu-id="c0052-107">Deletes a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0052-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0052-108">Prerequisites</span></span>
<span data-ttu-id="c0052-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0052-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0052-111">Permission type</span></span>|<span data-ttu-id="c0052-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0052-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0052-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0052-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0052-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0052-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c0052-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0052-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0052-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0052-116">Not supported.</span></span>|
|<span data-ttu-id="c0052-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0052-117">Application</span></span>|<span data-ttu-id="c0052-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0052-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0052-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0052-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c0052-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0052-120">Request headers</span></span>
|<span data-ttu-id="c0052-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0052-121">Header</span></span>|<span data-ttu-id="c0052-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0052-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0052-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0052-123">Authorization</span></span>|<span data-ttu-id="c0052-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0052-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0052-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0052-125">Accept</span></span>|<span data-ttu-id="c0052-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0052-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0052-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0052-127">Request body</span></span>
<span data-ttu-id="c0052-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0052-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0052-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0052-129">Response</span></span>
<span data-ttu-id="c0052-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0052-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0052-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0052-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0052-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0052-132">Request</span></span>
<span data-ttu-id="c0052-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0052-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

### <a name="response"></a><span data-ttu-id="c0052-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0052-134">Response</span></span>
<span data-ttu-id="c0052-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0052-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



