---
title: Lista embeddedSIMActivationCodePoolAssignments
description: Lista as propriedades e os relacionamentos dos objetos embeddedSIMActivationCodePoolAssignment.
author: tfitzmac
ms.openlocfilehash: 798701e538d1eabe7d49350efdb16777deee3dea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352924"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="9d39c-103">Lista embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="9d39c-103">List embeddedSIMActivationCodePoolAssignments</span></span>

> <span data-ttu-id="9d39c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d39c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d39c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d39c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d39c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9d39c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d39c-107">Lista as propriedades e os relacionamentos dos objetos [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9d39c-107">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d39c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d39c-108">Prerequisites</span></span>
<span data-ttu-id="9d39c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d39c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d39c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d39c-111">Permission type</span></span>|<span data-ttu-id="9d39c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d39c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d39c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d39c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d39c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d39c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9d39c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d39c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d39c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d39c-116">Not supported.</span></span>|
|<span data-ttu-id="9d39c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d39c-117">Application</span></span>|<span data-ttu-id="9d39c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d39c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d39c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d39c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9d39c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d39c-120">Request headers</span></span>
|<span data-ttu-id="9d39c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d39c-121">Header</span></span>|<span data-ttu-id="9d39c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d39c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d39c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d39c-123">Authorization</span></span>|<span data-ttu-id="9d39c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d39c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d39c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d39c-125">Accept</span></span>|<span data-ttu-id="9d39c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d39c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d39c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d39c-127">Request body</span></span>
<span data-ttu-id="9d39c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d39c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d39c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d39c-129">Response</span></span>
<span data-ttu-id="9d39c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d39c-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d39c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d39c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d39c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d39c-132">Request</span></span>
<span data-ttu-id="9d39c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d39c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="9d39c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d39c-134">Response</span></span>
<span data-ttu-id="9d39c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d39c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





