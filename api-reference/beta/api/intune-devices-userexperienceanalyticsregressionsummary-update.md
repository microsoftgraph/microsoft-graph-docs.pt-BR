---
title: Atualizar userExperienceAnalyticsRegressionSummary
description: Atualiza as propriedades de um objeto userExperienceAnalyticsRegressionSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d16184b9a44ea167d3e8932ddde14c2c9e36209
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047459"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="cac28-103">Atualizar userExperienceAnalyticsRegressionSummary</span><span class="sxs-lookup"><span data-stu-id="cac28-103">Update userExperienceAnalyticsRegressionSummary</span></span>

<span data-ttu-id="cac28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cac28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cac28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cac28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cac28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cac28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cac28-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cac28-107">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cac28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cac28-108">Prerequisites</span></span>
<span data-ttu-id="cac28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cac28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cac28-111">Permission type</span></span>|<span data-ttu-id="cac28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cac28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cac28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cac28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cac28-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac28-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cac28-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cac28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cac28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cac28-116">Not supported.</span></span>|
|<span data-ttu-id="cac28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cac28-117">Application</span></span>|<span data-ttu-id="cac28-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac28-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cac28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cac28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="cac28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cac28-120">Request headers</span></span>
|<span data-ttu-id="cac28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cac28-121">Header</span></span>|<span data-ttu-id="cac28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cac28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cac28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cac28-123">Authorization</span></span>|<span data-ttu-id="cac28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cac28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cac28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cac28-125">Accept</span></span>|<span data-ttu-id="cac28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cac28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cac28-127">Request body</span></span>
<span data-ttu-id="cac28-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cac28-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="cac28-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cac28-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="cac28-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cac28-130">Property</span></span>|<span data-ttu-id="cac28-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cac28-131">Type</span></span>|<span data-ttu-id="cac28-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cac28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac28-133">id</span><span class="sxs-lookup"><span data-stu-id="cac28-133">id</span></span>|<span data-ttu-id="cac28-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cac28-134">String</span></span>|<span data-ttu-id="cac28-135">O identificador exclusivo do Resumo de regressão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cac28-135">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="cac28-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cac28-136">Response</span></span>
<span data-ttu-id="cac28-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cac28-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac28-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cac28-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cac28-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cac28-139">Request</span></span>
<span data-ttu-id="cac28-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cac28-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="cac28-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cac28-141">Response</span></span>
<span data-ttu-id="cac28-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cac28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```






