---
title: Atualizar windowsInformationProtectionNetworkLearningSummary
description: Atualizar as propriedades de um objeto windowsInformationProtectionNetworkLearningSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05c59d3bc28f5a0c29a33f1a0046b18331f46570
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409220"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="2bf78-103">Atualizar windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="2bf78-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="2bf78-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2bf78-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2bf78-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2bf78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bf78-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2bf78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bf78-107">Atualizar as propriedades de um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2bf78-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bf78-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bf78-108">Prerequisites</span></span>
<span data-ttu-id="2bf78-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2bf78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2bf78-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bf78-111">Permission type</span></span>|<span data-ttu-id="2bf78-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bf78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bf78-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bf78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bf78-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bf78-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bf78-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bf78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bf78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bf78-116">Not supported.</span></span>|
|<span data-ttu-id="2bf78-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bf78-117">Application</span></span>|<span data-ttu-id="2bf78-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bf78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bf78-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bf78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="2bf78-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf78-120">Request headers</span></span>
|<span data-ttu-id="2bf78-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bf78-121">Header</span></span>|<span data-ttu-id="2bf78-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2bf78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bf78-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bf78-123">Authorization</span></span>|<span data-ttu-id="2bf78-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bf78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bf78-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bf78-125">Accept</span></span>|<span data-ttu-id="2bf78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bf78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bf78-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf78-127">Request body</span></span>
<span data-ttu-id="2bf78-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2bf78-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="2bf78-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2bf78-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="2bf78-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bf78-130">Property</span></span>|<span data-ttu-id="2bf78-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bf78-131">Type</span></span>|<span data-ttu-id="2bf78-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bf78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bf78-133">id</span><span class="sxs-lookup"><span data-stu-id="2bf78-133">id</span></span>|<span data-ttu-id="2bf78-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bf78-134">String</span></span>|<span data-ttu-id="2bf78-135">Identificador exclusivo de WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2bf78-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="2bf78-136">url</span><span class="sxs-lookup"><span data-stu-id="2bf78-136">url</span></span>|<span data-ttu-id="2bf78-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bf78-137">String</span></span>|<span data-ttu-id="2bf78-138">Url do site</span><span class="sxs-lookup"><span data-stu-id="2bf78-138">Website url</span></span>|
|<span data-ttu-id="2bf78-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2bf78-139">deviceCount</span></span>|<span data-ttu-id="2bf78-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2bf78-140">Int32</span></span>|<span data-ttu-id="2bf78-141">Contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="2bf78-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="2bf78-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf78-142">Response</span></span>
<span data-ttu-id="2bf78-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bf78-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bf78-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bf78-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bf78-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf78-145">Request</span></span>
<span data-ttu-id="2bf78-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bf78-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2bf78-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf78-147">Response</span></span>
<span data-ttu-id="2bf78-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bf78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




