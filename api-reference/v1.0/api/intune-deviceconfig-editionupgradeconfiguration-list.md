---
title: Listar editionUpgradeConfigurations
description: Listar propriedades e relações dos objetos editionUpgradeConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04742d586039bf341eee75013100bb74db0e38f3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753892"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="34dbb-103">Listar editionUpgradeConfigurations</span><span class="sxs-lookup"><span data-stu-id="34dbb-103">List editionUpgradeConfigurations</span></span>

<span data-ttu-id="34dbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34dbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34dbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34dbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34dbb-106">Listar propriedades e relações dos objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34dbb-106">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34dbb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34dbb-107">Prerequisites</span></span>
<span data-ttu-id="34dbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34dbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34dbb-110">Permission type</span></span>|<span data-ttu-id="34dbb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34dbb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34dbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34dbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34dbb-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34dbb-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34dbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34dbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34dbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34dbb-115">Not supported.</span></span>|
|<span data-ttu-id="34dbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34dbb-116">Application</span></span>|<span data-ttu-id="34dbb-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34dbb-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34dbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34dbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34dbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34dbb-119">Request headers</span></span>
|<span data-ttu-id="34dbb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34dbb-120">Header</span></span>|<span data-ttu-id="34dbb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34dbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34dbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34dbb-122">Authorization</span></span>|<span data-ttu-id="34dbb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34dbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34dbb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34dbb-124">Accept</span></span>|<span data-ttu-id="34dbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34dbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34dbb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34dbb-126">Request body</span></span>
<span data-ttu-id="34dbb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34dbb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34dbb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="34dbb-128">Response</span></span>
<span data-ttu-id="34dbb-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34dbb-129">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34dbb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34dbb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="34dbb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34dbb-131">Request</span></span>
<span data-ttu-id="34dbb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34dbb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="34dbb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="34dbb-133">Response</span></span>
<span data-ttu-id="34dbb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34dbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




