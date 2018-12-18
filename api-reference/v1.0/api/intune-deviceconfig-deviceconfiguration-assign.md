---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 4a7eea2b7fe321536add6dcbe458d1b3d7ec6e88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355395"
---
# <a name="assign-action"></a><span data-ttu-id="2df5e-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="2df5e-103">assign action</span></span>

> <span data-ttu-id="2df5e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2df5e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df5e-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2df5e-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df5e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2df5e-106">Prerequisites</span></span>
<span data-ttu-id="2df5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df5e-109">Permission type</span></span>|<span data-ttu-id="2df5e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2df5e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df5e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2df5e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df5e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2df5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df5e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df5e-114">Not supported.</span></span>|
|<span data-ttu-id="2df5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df5e-115">Application</span></span>|<span data-ttu-id="2df5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df5e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df5e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2df5e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df5e-118">Request headers</span></span>
|<span data-ttu-id="2df5e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2df5e-119">Header</span></span>|<span data-ttu-id="2df5e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2df5e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df5e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df5e-121">Authorization</span></span>|<span data-ttu-id="2df5e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df5e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df5e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2df5e-123">Accept</span></span>|<span data-ttu-id="2df5e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2df5e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df5e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df5e-125">Request body</span></span>
<span data-ttu-id="2df5e-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2df5e-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2df5e-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2df5e-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2df5e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2df5e-128">Property</span></span>|<span data-ttu-id="2df5e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df5e-129">Type</span></span>|<span data-ttu-id="2df5e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df5e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df5e-131">assignments</span><span class="sxs-lookup"><span data-stu-id="2df5e-131">assignments</span></span>|<span data-ttu-id="2df5e-132">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2df5e-132">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2df5e-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2df5e-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2df5e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df5e-134">Response</span></span>
<span data-ttu-id="2df5e-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df5e-135">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df5e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df5e-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df5e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df5e-137">Request</span></span>
<span data-ttu-id="2df5e-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df5e-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 277

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="2df5e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df5e-139">Response</span></span>
<span data-ttu-id="2df5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



