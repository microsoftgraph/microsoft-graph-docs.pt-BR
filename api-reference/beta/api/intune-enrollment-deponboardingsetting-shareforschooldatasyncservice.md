---
title: Ação shareForSchoolDataSyncService
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0b7f152d472524216e004108cadb0387b1a277c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167008"
---
# <a name="shareforschooldatasyncservice-action"></a><span data-ttu-id="42d10-103">Ação shareForSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="42d10-103">shareForSchoolDataSyncService action</span></span>

> <span data-ttu-id="42d10-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42d10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42d10-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d10-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42d10-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42d10-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42d10-107">Prerequisites</span></span>
<span data-ttu-id="42d10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42d10-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42d10-110">Permission type</span></span>|<span data-ttu-id="42d10-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42d10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42d10-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42d10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42d10-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d10-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42d10-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42d10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42d10-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d10-115">Not supported.</span></span>|
|<span data-ttu-id="42d10-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d10-116">Application</span></span>|<span data-ttu-id="42d10-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42d10-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42d10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/shareForSchoolDataSyncService
```

## <a name="request-headers"></a><span data-ttu-id="42d10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42d10-119">Request headers</span></span>
|<span data-ttu-id="42d10-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42d10-120">Header</span></span>|<span data-ttu-id="42d10-121">Valor</span><span class="sxs-lookup"><span data-stu-id="42d10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42d10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42d10-122">Authorization</span></span>|<span data-ttu-id="42d10-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42d10-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42d10-124">Accept</span></span>|<span data-ttu-id="42d10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42d10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42d10-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42d10-126">Request body</span></span>
<span data-ttu-id="42d10-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42d10-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42d10-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d10-128">Response</span></span>
<span data-ttu-id="42d10-129">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42d10-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42d10-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42d10-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="42d10-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42d10-131">Request</span></span>
<span data-ttu-id="42d10-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d10-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/shareForSchoolDataSyncService
```

### <a name="response"></a><span data-ttu-id="42d10-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d10-133">Response</span></span>
<span data-ttu-id="42d10-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42d10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




