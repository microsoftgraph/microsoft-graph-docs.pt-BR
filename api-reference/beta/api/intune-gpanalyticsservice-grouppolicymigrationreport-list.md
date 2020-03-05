---
title: Listar groupPolicyMigrationReports
description: Listar Propriedades e relações dos objetos groupPolicyMigrationReport.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d87fe0defd35e5c0623951b8fb8c959248f07ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465482"
---
# <a name="list-grouppolicymigrationreports"></a><span data-ttu-id="eb2ef-103">Listar groupPolicyMigrationReports</span><span class="sxs-lookup"><span data-stu-id="eb2ef-103">List groupPolicyMigrationReports</span></span>

<span data-ttu-id="eb2ef-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb2ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb2ef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb2ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb2ef-107">Listar Propriedades e relações dos objetos [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="eb2ef-107">List properties and relationships of the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb2ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb2ef-108">Prerequisites</span></span>
<span data-ttu-id="eb2ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb2ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb2ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb2ef-111">Permission type</span></span>|<span data-ttu-id="eb2ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb2ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb2ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb2ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb2ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb2ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb2ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb2ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb2ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-116">Not supported.</span></span>|
|<span data-ttu-id="eb2ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb2ef-117">Application</span></span>|<span data-ttu-id="eb2ef-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb2ef-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb2ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb2ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="eb2ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2ef-120">Request headers</span></span>
|<span data-ttu-id="eb2ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb2ef-121">Header</span></span>|<span data-ttu-id="eb2ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eb2ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb2ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb2ef-123">Authorization</span></span>|<span data-ttu-id="eb2ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb2ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb2ef-125">Accept</span></span>|<span data-ttu-id="eb2ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb2ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb2ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2ef-127">Request body</span></span>
<span data-ttu-id="eb2ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb2ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb2ef-129">Response</span></span>
<span data-ttu-id="eb2ef-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb2ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb2ef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb2ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2ef-132">Request</span></span>
<span data-ttu-id="eb2ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
```

### <a name="response"></a><span data-ttu-id="eb2ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb2ef-134">Response</span></span>
<span data-ttu-id="eb2ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb2ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





