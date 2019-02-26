---
title: Listar deviceConfigurationAssignments
description: Listar propriedades e relações dos objetos deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c7903067f103c0e15c9136f511bba5ac9f84c7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252613"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="fb4ea-103">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="fb4ea-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="fb4ea-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb4ea-105">Listar propriedades e relações dos objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fb4ea-105">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb4ea-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb4ea-106">Prerequisites</span></span>
<span data-ttu-id="fb4ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb4ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fb4ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb4ea-109">Permission type</span></span>|<span data-ttu-id="fb4ea-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb4ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb4ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb4ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb4ea-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb4ea-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb4ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb4ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb4ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-114">Not supported.</span></span>|
|<span data-ttu-id="fb4ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb4ea-115">Application</span></span>|<span data-ttu-id="fb4ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb4ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb4ea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="fb4ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4ea-118">Request headers</span></span>
|<span data-ttu-id="fb4ea-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb4ea-119">Header</span></span>|<span data-ttu-id="fb4ea-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fb4ea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb4ea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb4ea-121">Authorization</span></span>|<span data-ttu-id="fb4ea-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb4ea-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb4ea-123">Accept</span></span>|<span data-ttu-id="fb4ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fb4ea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb4ea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4ea-125">Request body</span></span>
<span data-ttu-id="fb4ea-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb4ea-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb4ea-127">Response</span></span>
<span data-ttu-id="fb4ea-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb4ea-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb4ea-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb4ea-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb4ea-130">Request</span></span>
<span data-ttu-id="fb4ea-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="fb4ea-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb4ea-132">Response</span></span>
<span data-ttu-id="fb4ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb4ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



