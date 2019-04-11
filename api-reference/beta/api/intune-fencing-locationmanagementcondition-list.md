---
title: Listar locationManagementConditions
description: Listar Propriedades e relações dos objetos locationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6987f4fd130efa44ffcbfd45b8eb31d4263d7f79
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807802"
---
# <a name="list-locationmanagementconditions"></a><span data-ttu-id="97474-103">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="97474-103">List locationManagementConditions</span></span>

> <span data-ttu-id="97474-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97474-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97474-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97474-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97474-106">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="97474-106">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97474-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97474-107">Prerequisites</span></span>
<span data-ttu-id="97474-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97474-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97474-110">Permission type</span></span>|<span data-ttu-id="97474-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97474-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97474-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97474-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97474-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97474-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97474-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97474-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97474-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97474-115">Not supported.</span></span>|
|<span data-ttu-id="97474-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97474-116">Application</span></span>|<span data-ttu-id="97474-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97474-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97474-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97474-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="97474-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97474-119">Request headers</span></span>
|<span data-ttu-id="97474-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97474-120">Header</span></span>|<span data-ttu-id="97474-121">Valor</span><span class="sxs-lookup"><span data-stu-id="97474-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97474-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="97474-122">Authorization</span></span>|<span data-ttu-id="97474-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97474-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97474-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97474-124">Accept</span></span>|<span data-ttu-id="97474-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97474-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97474-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97474-126">Request body</span></span>
<span data-ttu-id="97474-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97474-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97474-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="97474-128">Response</span></span>
<span data-ttu-id="97474-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97474-129">If successful, this method returns a `200 OK` response code and a collection of [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97474-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97474-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97474-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97474-131">Request</span></span>
<span data-ttu-id="97474-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97474-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="97474-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="97474-133">Response</span></span>
<span data-ttu-id="97474-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97474-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.locationManagementCondition",
      "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





