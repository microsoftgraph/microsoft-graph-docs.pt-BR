---
title: Listar groupPolicyMigrationReports
description: Listar Propriedades e relações dos objetos groupPolicyMigrationReport.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5211f12f0f7a8b55a2942236c522cc04c322c24c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804615"
---
# <a name="list-grouppolicymigrationreports"></a><span data-ttu-id="0ee82-103">Listar groupPolicyMigrationReports</span><span class="sxs-lookup"><span data-stu-id="0ee82-103">List groupPolicyMigrationReports</span></span>

> <span data-ttu-id="0ee82-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ee82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ee82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee82-106">Listar Propriedades e relações dos objetos [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="0ee82-106">List properties and relationships of the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee82-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ee82-107">Prerequisites</span></span>
<span data-ttu-id="0ee82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee82-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ee82-110">Permission type</span></span>|<span data-ttu-id="0ee82-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ee82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee82-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ee82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee82-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee82-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ee82-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ee82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee82-115">Not supported.</span></span>|
|<span data-ttu-id="0ee82-116">Application</span><span class="sxs-lookup"><span data-stu-id="0ee82-116">Application</span></span>|<span data-ttu-id="0ee82-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee82-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee82-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="0ee82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee82-119">Request headers</span></span>
|<span data-ttu-id="0ee82-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ee82-120">Header</span></span>|<span data-ttu-id="0ee82-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ee82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee82-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ee82-122">Authorization</span></span>|<span data-ttu-id="0ee82-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ee82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee82-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ee82-124">Accept</span></span>|<span data-ttu-id="0ee82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee82-126">Request body</span></span>
<span data-ttu-id="0ee82-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ee82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee82-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee82-128">Response</span></span>
<span data-ttu-id="0ee82-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee82-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee82-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ee82-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee82-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee82-131">Request</span></span>
<span data-ttu-id="0ee82-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ee82-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
```

### <a name="response"></a><span data-ttu-id="0ee82-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee82-133">Response</span></span>
<span data-ttu-id="0ee82-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ee82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 805

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
      "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
      "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
      "displayName": "Display Name value",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
      "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
      "migrationReadiness": "partial",
      "targetedInActiveDirectory": true,
      "totalSettingsCount": 2,
      "supportedSettingsCount": 6,
      "supportedSettingsPercent": 8
    }
  ]
}
```




