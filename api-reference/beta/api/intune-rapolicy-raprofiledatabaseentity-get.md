---
title: Obter raProfileDatabaseEntity
description: Leia as propriedades e as relações do objeto raProfileDatabaseEntity.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0dbd34afd108a50a5e91aac414cc19ecd86282
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124176"
---
# <a name="get-raprofiledatabaseentity"></a><span data-ttu-id="f43b7-103">Obter raProfileDatabaseEntity</span><span class="sxs-lookup"><span data-stu-id="f43b7-103">Get raProfileDatabaseEntity</span></span>

<span data-ttu-id="f43b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f43b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f43b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f43b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f43b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f43b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f43b7-107">Leia as propriedades e as relações do objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f43b7-107">Read properties and relationships of the [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f43b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f43b7-108">Prerequisites</span></span>
<span data-ttu-id="f43b7-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f43b7-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f43b7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f43b7-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f43b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f43b7-111">Permission type</span></span>|<span data-ttu-id="f43b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f43b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f43b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f43b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f43b7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f43b7-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f43b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f43b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f43b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f43b7-116">Not supported.</span></span>|
|<span data-ttu-id="f43b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f43b7-117">Application</span></span>|<span data-ttu-id="f43b7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f43b7-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f43b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f43b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f43b7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f43b7-120">Optional query parameters</span></span>
<span data-ttu-id="f43b7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f43b7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f43b7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f43b7-122">Request headers</span></span>
|<span data-ttu-id="f43b7-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f43b7-123">Header</span></span>|<span data-ttu-id="f43b7-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f43b7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f43b7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f43b7-125">Authorization</span></span>|<span data-ttu-id="f43b7-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f43b7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f43b7-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f43b7-127">Accept</span></span>|<span data-ttu-id="f43b7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f43b7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f43b7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f43b7-129">Request body</span></span>
<span data-ttu-id="f43b7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f43b7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f43b7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43b7-131">Response</span></span>
<span data-ttu-id="f43b7-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f43b7-132">If successful, this method returns a `200 OK` response code and [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f43b7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f43b7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f43b7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f43b7-134">Request</span></span>
<span data-ttu-id="f43b7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f43b7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a><span data-ttu-id="f43b7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43b7-136">Response</span></span>
<span data-ttu-id="f43b7-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f43b7-137">Here is an example of the response.</span></span> <span data-ttu-id="f43b7-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f43b7-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f43b7-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f43b7-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "value": {
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
}
```



