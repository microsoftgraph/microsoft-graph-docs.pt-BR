---
title: Listar deviceConfigurationAssignments
description: Listar propriedades e relações dos objetos deviceConfigurationAssignment.
ms.openlocfilehash: 6d8407f17d5ef1cb5ac771fd86bd4365d9e92876
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006270"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="c0c75-103">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c0c75-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="c0c75-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c0c75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0c75-105">Listar propriedades e relações dos objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0c75-105">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0c75-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0c75-106">Prerequisites</span></span>
<span data-ttu-id="c0c75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0c75-109">Permission type</span></span>|<span data-ttu-id="c0c75-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0c75-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0c75-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0c75-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0c75-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0c75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0c75-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0c75-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c75-114">Not supported.</span></span>|
|<span data-ttu-id="c0c75-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0c75-115">Application</span></span>|<span data-ttu-id="c0c75-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c75-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c75-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c75-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c0c75-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c75-118">Request headers</span></span>
|<span data-ttu-id="c0c75-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0c75-119">Header</span></span>|<span data-ttu-id="c0c75-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c0c75-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0c75-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0c75-121">Authorization</span></span>|<span data-ttu-id="c0c75-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0c75-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0c75-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c0c75-123">Accept</span></span>|<span data-ttu-id="c0c75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c75-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c75-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c75-125">Request body</span></span>
<span data-ttu-id="c0c75-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0c75-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c75-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c75-127">Response</span></span>
<span data-ttu-id="c0c75-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0c75-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c75-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0c75-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0c75-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c75-130">Request</span></span>
<span data-ttu-id="c0c75-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0c75-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="c0c75-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c75-132">Response</span></span>
<span data-ttu-id="c0c75-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0c75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



