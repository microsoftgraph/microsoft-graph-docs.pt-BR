---
title: Listar raProfileDatabaseEntities
description: Listar Propriedades e relações dos objetos raProfileDatabaseEntity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca8a822b0a79d1e9144261b6cd2f219ee01cbcbb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124175"
---
# <a name="list-raprofiledatabaseentities"></a><span data-ttu-id="4b3b6-103">Listar raProfileDatabaseEntities</span><span class="sxs-lookup"><span data-stu-id="4b3b6-103">List raProfileDatabaseEntities</span></span>

<span data-ttu-id="4b3b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b3b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b3b6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b3b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b3b6-107">Listar Propriedades e relações dos objetos [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3b6-107">List properties and relationships of the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b3b6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b3b6-108">Prerequisites</span></span>
<span data-ttu-id="4b3b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b3b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b3b6-111">Permission type</span></span>|<span data-ttu-id="4b3b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b3b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b3b6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b3b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b3b6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3b6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4b3b6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b3b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b3b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-116">Not supported.</span></span>|
|<span data-ttu-id="4b3b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b3b6-117">Application</span></span>|<span data-ttu-id="4b3b6-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b3b6-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b3b6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b3b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities
```

## <a name="request-headers"></a><span data-ttu-id="4b3b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3b6-120">Request headers</span></span>
|<span data-ttu-id="4b3b6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b3b6-121">Header</span></span>|<span data-ttu-id="4b3b6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b3b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b3b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b3b6-123">Authorization</span></span>|<span data-ttu-id="4b3b6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b3b6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b3b6-125">Accept</span></span>|<span data-ttu-id="4b3b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b3b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b3b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3b6-127">Request body</span></span>
<span data-ttu-id="4b3b6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b3b6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b3b6-129">Response</span></span>
<span data-ttu-id="4b3b6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-130">If successful, this method returns a `200 OK` response code and a collection of [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b3b6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b3b6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b3b6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b3b6-132">Request</span></span>
<span data-ttu-id="4b3b6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities
```

### <a name="response"></a><span data-ttu-id="4b3b6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b3b6-134">Response</span></span>
<span data-ttu-id="4b3b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b3b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 908

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
      "version": 7,
      "isDeleted": true,
      "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
      "displayName": "Display Name value",
      "linkedProfileIds": [
        "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
      ],
      "profileTypeName": "Profile Type Name value",
      "profileBody": "Profile Body value",
      "profileBodyHash": "Profile Body Hash value",
      "platformType": 12,
      "transformedProfileBody": "Transformed Profile Body value",
      "transformedProfileBodyHash": "Transformed Profile Body Hash value",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "profileId": "6389d896-d896-6389-96d8-896396d88963",
      "eTag": "ETag value",
      "schemaVersion": "betaStart",
      "lastModified": "2017-01-01T00:03:14.6651031-08:00"
    }
  ]
}
```



