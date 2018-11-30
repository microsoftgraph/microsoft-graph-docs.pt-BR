---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
ms.openlocfilehash: ade11aa7dfdbe9f189923ad470d411e19a50fb51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037879"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="3d29c-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="3d29c-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="3d29c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3d29c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d29c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3d29c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d29c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d29c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d29c-107">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3d29c-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d29c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d29c-108">Prerequisites</span></span>
<span data-ttu-id="3d29c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d29c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d29c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d29c-111">Permission type</span></span>|<span data-ttu-id="3d29c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d29c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d29c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d29c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d29c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d29c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d29c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d29c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d29c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d29c-116">Not supported.</span></span>|
|<span data-ttu-id="3d29c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d29c-117">Application</span></span>|<span data-ttu-id="3d29c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d29c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d29c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d29c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3d29c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d29c-120">Request headers</span></span>
|<span data-ttu-id="3d29c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d29c-121">Header</span></span>|<span data-ttu-id="3d29c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3d29c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d29c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d29c-123">Authorization</span></span>|<span data-ttu-id="3d29c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d29c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d29c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d29c-125">Accept</span></span>|<span data-ttu-id="3d29c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d29c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d29c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d29c-127">Request body</span></span>
<span data-ttu-id="3d29c-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3d29c-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="3d29c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3d29c-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="3d29c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d29c-130">Property</span></span>|<span data-ttu-id="3d29c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d29c-131">Type</span></span>|<span data-ttu-id="3d29c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d29c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d29c-133">id</span><span class="sxs-lookup"><span data-stu-id="3d29c-133">id</span></span>|<span data-ttu-id="3d29c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d29c-134">String</span></span>|<span data-ttu-id="3d29c-135">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="3d29c-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="3d29c-136">url</span><span class="sxs-lookup"><span data-stu-id="3d29c-136">url</span></span>|<span data-ttu-id="3d29c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d29c-137">String</span></span>|<span data-ttu-id="3d29c-138">Url do site</span><span class="sxs-lookup"><span data-stu-id="3d29c-138">Website url</span></span>|
|<span data-ttu-id="3d29c-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3d29c-139">deviceCount</span></span>|<span data-ttu-id="3d29c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3d29c-140">Int32</span></span>|<span data-ttu-id="3d29c-141">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3d29c-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="3d29c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d29c-142">Response</span></span>
<span data-ttu-id="3d29c-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d29c-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d29c-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d29c-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d29c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d29c-145">Request</span></span>
<span data-ttu-id="3d29c-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d29c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="3d29c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d29c-147">Response</span></span>
<span data-ttu-id="3d29c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d29c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





