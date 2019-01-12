---
title: Criar windowsInformationProtectionNetworkLearningSummary
description: Criar um novo objeto windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 59b55111a022c1172abb9ab9f65ccf23e153c8cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915526"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="11778-103">Criar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="11778-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="11778-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11778-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11778-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11778-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11778-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="11778-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11778-107">Criar um novo objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="11778-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11778-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11778-108">Prerequisites</span></span>
<span data-ttu-id="11778-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11778-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11778-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11778-111">Permission type</span></span>|<span data-ttu-id="11778-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11778-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11778-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11778-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11778-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11778-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11778-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11778-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11778-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11778-116">Not supported.</span></span>|
|<span data-ttu-id="11778-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11778-117">Application</span></span>|<span data-ttu-id="11778-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11778-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11778-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11778-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="11778-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11778-120">Request headers</span></span>
|<span data-ttu-id="11778-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11778-121">Header</span></span>|<span data-ttu-id="11778-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11778-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11778-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11778-123">Authorization</span></span>|<span data-ttu-id="11778-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11778-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11778-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11778-125">Accept</span></span>|<span data-ttu-id="11778-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11778-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11778-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11778-127">Request body</span></span>
<span data-ttu-id="11778-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="11778-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="11778-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="11778-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="11778-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11778-130">Property</span></span>|<span data-ttu-id="11778-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11778-131">Type</span></span>|<span data-ttu-id="11778-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11778-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11778-133">id</span><span class="sxs-lookup"><span data-stu-id="11778-133">id</span></span>|<span data-ttu-id="11778-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11778-134">String</span></span>|<span data-ttu-id="11778-135">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="11778-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="11778-136">url</span><span class="sxs-lookup"><span data-stu-id="11778-136">url</span></span>|<span data-ttu-id="11778-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11778-137">String</span></span>|<span data-ttu-id="11778-138">Url do site</span><span class="sxs-lookup"><span data-stu-id="11778-138">Website url</span></span>|
|<span data-ttu-id="11778-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="11778-139">deviceCount</span></span>|<span data-ttu-id="11778-140">Int32</span><span class="sxs-lookup"><span data-stu-id="11778-140">Int32</span></span>|<span data-ttu-id="11778-141">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="11778-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="11778-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="11778-142">Response</span></span>
<span data-ttu-id="11778-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11778-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11778-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11778-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="11778-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11778-145">Request</span></span>
<span data-ttu-id="11778-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11778-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="11778-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="11778-147">Response</span></span>
<span data-ttu-id="11778-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11778-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```





