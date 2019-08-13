---
title: Listar networkIPv6ConfigurationManagementConditions
description: Listar Propriedades e relações dos objetos networkIPv6ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a0aa5745baa7771e8370b62446d8949184857666
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355427"
---
# <a name="list-networkipv6configurationmanagementconditions"></a><span data-ttu-id="97536-103">Listar networkIPv6ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="97536-103">List networkIPv6ConfigurationManagementConditions</span></span>

> <span data-ttu-id="97536-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97536-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97536-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97536-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97536-106">Listar Propriedades e relações dos objetos [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="97536-106">List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97536-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97536-107">Prerequisites</span></span>
<span data-ttu-id="97536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97536-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97536-110">Permission type</span></span>|<span data-ttu-id="97536-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97536-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97536-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97536-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97536-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97536-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97536-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97536-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97536-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97536-115">Not supported.</span></span>|
|<span data-ttu-id="97536-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97536-116">Application</span></span>|<span data-ttu-id="97536-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97536-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97536-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97536-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="97536-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97536-119">Request headers</span></span>
|<span data-ttu-id="97536-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97536-120">Header</span></span>|<span data-ttu-id="97536-121">Valor</span><span class="sxs-lookup"><span data-stu-id="97536-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97536-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="97536-122">Authorization</span></span>|<span data-ttu-id="97536-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97536-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97536-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97536-124">Accept</span></span>|<span data-ttu-id="97536-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97536-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97536-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97536-126">Request body</span></span>
<span data-ttu-id="97536-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97536-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97536-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="97536-128">Response</span></span>
<span data-ttu-id="97536-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97536-129">If successful, this method returns a `200 OK` response code and a collection of [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97536-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97536-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97536-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97536-131">Request</span></span>
<span data-ttu-id="97536-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97536-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="97536-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="97536-133">Response</span></span>
<span data-ttu-id="97536-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
      "id": "25811206-1206-2581-0612-812506128125",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "ipV6Prefix": "Ip V6Prefix value",
      "ipV6Gateway": "Ip V6Gateway value",
      "ipV6DNSServerList": [
        "Ip V6DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```






