---
title: Listar editionUpgradeConfigurations
description: Listar propriedades e relações dos objetos editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae89e5933bbd1ee492daa99a2f53972c292d3842
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966619"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="c67dd-103">Listar editionUpgradeConfigurations</span><span class="sxs-lookup"><span data-stu-id="c67dd-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="c67dd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c67dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c67dd-105">Listar propriedades e relações dos objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c67dd-105">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c67dd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c67dd-106">Prerequisites</span></span>
<span data-ttu-id="c67dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c67dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c67dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c67dd-109">Permission type</span></span>|<span data-ttu-id="c67dd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c67dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c67dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c67dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c67dd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c67dd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c67dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c67dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c67dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67dd-114">Not supported.</span></span>|
|<span data-ttu-id="c67dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c67dd-115">Application</span></span>|<span data-ttu-id="c67dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c67dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c67dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c67dd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c67dd-118">Request headers</span></span>
|<span data-ttu-id="c67dd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c67dd-119">Header</span></span>|<span data-ttu-id="c67dd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c67dd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c67dd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c67dd-121">Authorization</span></span>|<span data-ttu-id="c67dd-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c67dd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c67dd-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c67dd-123">Accept</span></span>|<span data-ttu-id="c67dd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c67dd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c67dd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c67dd-125">Request body</span></span>
<span data-ttu-id="c67dd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c67dd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c67dd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c67dd-127">Response</span></span>
<span data-ttu-id="c67dd-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c67dd-128">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c67dd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c67dd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c67dd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c67dd-130">Request</span></span>
<span data-ttu-id="c67dd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c67dd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c67dd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c67dd-132">Response</span></span>
<span data-ttu-id="c67dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c67dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



