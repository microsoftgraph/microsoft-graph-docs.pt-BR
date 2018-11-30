---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
ms.openlocfilehash: a40cd274b03cd9efeddf053f2e6ed4d81b836752
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007486"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="18970-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="18970-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="18970-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18970-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18970-105">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="18970-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18970-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18970-106">Prerequisites</span></span>
<span data-ttu-id="18970-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18970-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18970-109">Permission type</span></span>|<span data-ttu-id="18970-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18970-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18970-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18970-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18970-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18970-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18970-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18970-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18970-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18970-114">Not supported.</span></span>|
|<span data-ttu-id="18970-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18970-115">Application</span></span>|<span data-ttu-id="18970-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18970-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18970-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18970-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="18970-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18970-118">Request headers</span></span>
|<span data-ttu-id="18970-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18970-119">Header</span></span>|<span data-ttu-id="18970-120">Valor</span><span class="sxs-lookup"><span data-stu-id="18970-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18970-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="18970-121">Authorization</span></span>|<span data-ttu-id="18970-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18970-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18970-123">Accept</span><span class="sxs-lookup"><span data-stu-id="18970-123">Accept</span></span>|<span data-ttu-id="18970-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18970-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18970-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18970-125">Request body</span></span>
<span data-ttu-id="18970-126">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="18970-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="18970-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="18970-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="18970-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18970-128">Property</span></span>|<span data-ttu-id="18970-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="18970-129">Type</span></span>|<span data-ttu-id="18970-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="18970-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18970-131">id</span><span class="sxs-lookup"><span data-stu-id="18970-131">id</span></span>|<span data-ttu-id="18970-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18970-132">String</span></span>|<span data-ttu-id="18970-133">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="18970-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="18970-134">url</span><span class="sxs-lookup"><span data-stu-id="18970-134">url</span></span>|<span data-ttu-id="18970-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18970-135">String</span></span>|<span data-ttu-id="18970-136">Url do site</span><span class="sxs-lookup"><span data-stu-id="18970-136">Website url</span></span>|
|<span data-ttu-id="18970-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="18970-137">deviceCount</span></span>|<span data-ttu-id="18970-138">Int32</span><span class="sxs-lookup"><span data-stu-id="18970-138">Int32</span></span>|<span data-ttu-id="18970-139">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="18970-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="18970-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="18970-140">Response</span></span>
<span data-ttu-id="18970-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18970-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18970-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18970-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="18970-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18970-143">Request</span></span>
<span data-ttu-id="18970-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18970-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18970-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="18970-145">Response</span></span>
<span data-ttu-id="18970-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18970-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



