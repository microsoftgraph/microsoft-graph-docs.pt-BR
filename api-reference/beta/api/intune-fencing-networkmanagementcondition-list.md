---
title: Lista networkManagementConditions
description: Lista as propriedades e os relacionamentos dos objetos networkManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bb9c623d46b41221ad34267c5770c67e39feda00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980094"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="688ed-103">Lista networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="688ed-103">List networkManagementConditions</span></span>

> <span data-ttu-id="688ed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="688ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="688ed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="688ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="688ed-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="688ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="688ed-107">Lista as propriedades e os relacionamentos dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="688ed-107">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="688ed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="688ed-108">Prerequisites</span></span>
<span data-ttu-id="688ed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="688ed-111">Permission type</span></span>|<span data-ttu-id="688ed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="688ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="688ed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="688ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="688ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="688ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="688ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="688ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="688ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="688ed-116">Not supported.</span></span>|
|<span data-ttu-id="688ed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="688ed-117">Application</span></span>|<span data-ttu-id="688ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="688ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="688ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="688ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="688ed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="688ed-120">Request headers</span></span>
|<span data-ttu-id="688ed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="688ed-121">Header</span></span>|<span data-ttu-id="688ed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="688ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="688ed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="688ed-123">Authorization</span></span>|<span data-ttu-id="688ed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="688ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="688ed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="688ed-125">Accept</span></span>|<span data-ttu-id="688ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="688ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="688ed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="688ed-127">Request body</span></span>
<span data-ttu-id="688ed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="688ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="688ed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="688ed-129">Response</span></span>
<span data-ttu-id="688ed-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="688ed-130">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688ed-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="688ed-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="688ed-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="688ed-132">Request</span></span>
<span data-ttu-id="688ed-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="688ed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="688ed-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="688ed-134">Response</span></span>
<span data-ttu-id="688ed-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="688ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkManagementCondition",
      "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
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





