---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4bdd0b00249828c7ae45aff68b04a2acf900c8d4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748928"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="7cd20-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7cd20-103">Update deviceManagement</span></span>

<span data-ttu-id="7cd20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cd20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cd20-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cd20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cd20-106">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7cd20-106">Update the properties of a [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cd20-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7cd20-107">Prerequisites</span></span>
<span data-ttu-id="7cd20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cd20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cd20-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cd20-110">Permission type</span></span>|<span data-ttu-id="7cd20-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cd20-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cd20-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cd20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cd20-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cd20-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cd20-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cd20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cd20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cd20-115">Not supported.</span></span>|
|<span data-ttu-id="7cd20-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cd20-116">Application</span></span>|<span data-ttu-id="7cd20-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cd20-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cd20-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="7cd20-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd20-119">Request headers</span></span>
|<span data-ttu-id="7cd20-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cd20-120">Header</span></span>|<span data-ttu-id="7cd20-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7cd20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cd20-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cd20-122">Authorization</span></span>|<span data-ttu-id="7cd20-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cd20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cd20-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cd20-124">Accept</span></span>|<span data-ttu-id="7cd20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cd20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cd20-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd20-126">Request body</span></span>
<span data-ttu-id="7cd20-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7cd20-127">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>

<span data-ttu-id="7cd20-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7cd20-128">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span></span>

|<span data-ttu-id="7cd20-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cd20-129">Property</span></span>|<span data-ttu-id="7cd20-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cd20-130">Type</span></span>|<span data-ttu-id="7cd20-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cd20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd20-132">id</span><span class="sxs-lookup"><span data-stu-id="7cd20-132">id</span></span>|<span data-ttu-id="7cd20-133">String</span><span class="sxs-lookup"><span data-stu-id="7cd20-133">String</span></span>|<span data-ttu-id="7cd20-134">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="7cd20-134">Unique Identifier</span></span>|
|<span data-ttu-id="7cd20-135">settings</span><span class="sxs-lookup"><span data-stu-id="7cd20-135">settings</span></span>|[<span data-ttu-id="7cd20-136">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="7cd20-136">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="7cd20-137">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="7cd20-137">Account level settings.</span></span>|
|<span data-ttu-id="7cd20-138">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="7cd20-138">intuneAccountId</span></span>|<span data-ttu-id="7cd20-139">Guid</span><span class="sxs-lookup"><span data-stu-id="7cd20-139">Guid</span></span>|<span data-ttu-id="7cd20-140">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="7cd20-140">Intune Account Id for given tenant</span></span>|



## <a name="response"></a><span data-ttu-id="7cd20-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd20-141">Response</span></span>
<span data-ttu-id="7cd20-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd20-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cd20-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cd20-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cd20-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd20-144">Request</span></span>
<span data-ttu-id="7cd20-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cd20-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "cf1549a1-49a1-cf15-a149-15cfa14915cf"
}
```

### <a name="response"></a><span data-ttu-id="7cd20-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd20-146">Response</span></span>
<span data-ttu-id="7cd20-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cd20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "cf1549a1-49a1-cf15-a149-15cfa14915cf"
}
```




