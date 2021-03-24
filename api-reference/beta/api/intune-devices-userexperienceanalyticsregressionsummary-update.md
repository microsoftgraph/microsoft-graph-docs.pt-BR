---
title: Atualizar userExperienceAnalyticsRegressionSummary
description: Atualize as propriedades de um objeto userExperienceAnalyticsRegressionSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2d2676d03751426a6524d28869300a185f7a4f9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146171"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="f9b28-103">Atualizar userExperienceAnalyticsRegressionSummary</span><span class="sxs-lookup"><span data-stu-id="f9b28-103">Update userExperienceAnalyticsRegressionSummary</span></span>

<span data-ttu-id="f9b28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9b28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9b28-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9b28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9b28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9b28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9b28-107">Atualize as propriedades de [um objeto userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)</span><span class="sxs-lookup"><span data-stu-id="f9b28-107">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9b28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9b28-108">Prerequisites</span></span>
<span data-ttu-id="f9b28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9b28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9b28-111">Permission type</span></span>|<span data-ttu-id="f9b28-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9b28-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9b28-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9b28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9b28-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b28-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9b28-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9b28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9b28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b28-116">Not supported.</span></span>|
|<span data-ttu-id="f9b28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9b28-117">Application</span></span>|<span data-ttu-id="f9b28-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b28-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9b28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="f9b28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b28-120">Request headers</span></span>
|<span data-ttu-id="f9b28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9b28-121">Header</span></span>|<span data-ttu-id="f9b28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9b28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9b28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9b28-123">Authorization</span></span>|<span data-ttu-id="f9b28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9b28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9b28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9b28-125">Accept</span></span>|<span data-ttu-id="f9b28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9b28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b28-127">Request body</span></span>
<span data-ttu-id="f9b28-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)</span><span class="sxs-lookup"><span data-stu-id="f9b28-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="f9b28-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f9b28-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="f9b28-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9b28-130">Property</span></span>|<span data-ttu-id="f9b28-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9b28-131">Type</span></span>|<span data-ttu-id="f9b28-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9b28-133">id</span><span class="sxs-lookup"><span data-stu-id="f9b28-133">id</span></span>|<span data-ttu-id="f9b28-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b28-134">String</span></span>|<span data-ttu-id="f9b28-135">O identificador exclusivo do resumo de regressão de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9b28-135">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="f9b28-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b28-136">Response</span></span>
<span data-ttu-id="f9b28-137">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b28-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b28-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9b28-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9b28-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b28-139">Request</span></span>
<span data-ttu-id="f9b28-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9b28-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="f9b28-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b28-141">Response</span></span>
<span data-ttu-id="f9b28-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9b28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```




