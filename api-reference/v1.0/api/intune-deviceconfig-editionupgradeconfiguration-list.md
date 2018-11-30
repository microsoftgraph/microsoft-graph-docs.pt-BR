---
title: Listar editionUpgradeConfigurations
description: Listar propriedades e relações dos objetos editionUpgradeConfiguration.
ms.openlocfilehash: 1b60625a37fb95fefc5748b4feef460341d9ebc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005973"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="8f6df-103">Listar editionUpgradeConfigurations</span><span class="sxs-lookup"><span data-stu-id="8f6df-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="8f6df-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f6df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f6df-105">Listar propriedades e relações dos objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f6df-105">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f6df-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f6df-106">Prerequisites</span></span>
<span data-ttu-id="8f6df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f6df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f6df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f6df-109">Permission type</span></span>|<span data-ttu-id="8f6df-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f6df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f6df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f6df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f6df-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f6df-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8f6df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f6df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f6df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f6df-114">Not supported.</span></span>|
|<span data-ttu-id="8f6df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f6df-115">Application</span></span>|<span data-ttu-id="8f6df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f6df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f6df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f6df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f6df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f6df-118">Request headers</span></span>
|<span data-ttu-id="8f6df-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f6df-119">Header</span></span>|<span data-ttu-id="8f6df-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8f6df-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f6df-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f6df-121">Authorization</span></span>|<span data-ttu-id="8f6df-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f6df-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f6df-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8f6df-123">Accept</span></span>|<span data-ttu-id="8f6df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f6df-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f6df-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f6df-125">Request body</span></span>
<span data-ttu-id="8f6df-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f6df-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f6df-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f6df-127">Response</span></span>
<span data-ttu-id="8f6df-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f6df-128">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f6df-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f6df-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f6df-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f6df-130">Request</span></span>
<span data-ttu-id="8f6df-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f6df-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8f6df-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f6df-132">Response</span></span>
<span data-ttu-id="8f6df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f6df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
      "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "licenseType": "licenseFile",
      "targetEdition": "windows10EnterpriseN",
      "license": "License value",
      "productKey": "Product Key value"
    }
  ]
}
```



