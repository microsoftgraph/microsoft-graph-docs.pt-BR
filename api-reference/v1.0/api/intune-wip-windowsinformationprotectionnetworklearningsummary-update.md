---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 663b13d803e1205de07dc2f8a1311c82f5376cb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830475"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="213e6-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="213e6-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="213e6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="213e6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="213e6-105">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="213e6-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="213e6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="213e6-106">Prerequisites</span></span>
<span data-ttu-id="213e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="213e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="213e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="213e6-109">Permission type</span></span>|<span data-ttu-id="213e6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="213e6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="213e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="213e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="213e6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213e6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="213e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="213e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="213e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="213e6-114">Not supported.</span></span>|
|<span data-ttu-id="213e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="213e6-115">Application</span></span>|<span data-ttu-id="213e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="213e6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="213e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="213e6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="213e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="213e6-118">Request headers</span></span>
|<span data-ttu-id="213e6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="213e6-119">Header</span></span>|<span data-ttu-id="213e6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="213e6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="213e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="213e6-121">Authorization</span></span>|<span data-ttu-id="213e6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="213e6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="213e6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="213e6-123">Accept</span></span>|<span data-ttu-id="213e6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="213e6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="213e6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="213e6-125">Request body</span></span>
<span data-ttu-id="213e6-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="213e6-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="213e6-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="213e6-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="213e6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="213e6-128">Property</span></span>|<span data-ttu-id="213e6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="213e6-129">Type</span></span>|<span data-ttu-id="213e6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="213e6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="213e6-131">id</span><span class="sxs-lookup"><span data-stu-id="213e6-131">id</span></span>|<span data-ttu-id="213e6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="213e6-132">String</span></span>|<span data-ttu-id="213e6-133">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="213e6-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="213e6-134">url</span><span class="sxs-lookup"><span data-stu-id="213e6-134">url</span></span>|<span data-ttu-id="213e6-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="213e6-135">String</span></span>|<span data-ttu-id="213e6-136">Url do site</span><span class="sxs-lookup"><span data-stu-id="213e6-136">Website url</span></span>|
|<span data-ttu-id="213e6-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="213e6-137">deviceCount</span></span>|<span data-ttu-id="213e6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="213e6-138">Int32</span></span>|<span data-ttu-id="213e6-139">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="213e6-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="213e6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="213e6-140">Response</span></span>
<span data-ttu-id="213e6-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="213e6-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="213e6-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="213e6-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="213e6-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="213e6-143">Request</span></span>
<span data-ttu-id="213e6-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="213e6-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="213e6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="213e6-145">Response</span></span>
<span data-ttu-id="213e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="213e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



