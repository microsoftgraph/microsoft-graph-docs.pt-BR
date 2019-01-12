---
title: Lista officeClientConfigurationAssignments
description: Lista as propriedades e os relacionamentos dos objetos officeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e0398e5fe9773171ce8ba5d12c456a287185cdf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954418"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="e8c49-103">Lista officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="e8c49-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="e8c49-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8c49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8c49-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8c49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8c49-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e8c49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8c49-107">Lista as propriedades e os relacionamentos dos objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e8c49-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8c49-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8c49-108">Prerequisites</span></span>
<span data-ttu-id="e8c49-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8c49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8c49-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8c49-111">Permission type</span></span>|<span data-ttu-id="e8c49-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8c49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8c49-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8c49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8c49-114">\* \* TODO: Determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="e8c49-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="e8c49-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8c49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8c49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8c49-116">Not supported.</span></span>|
|<span data-ttu-id="e8c49-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8c49-117">Application</span></span>|<span data-ttu-id="e8c49-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8c49-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8c49-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8c49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e8c49-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8c49-120">Request headers</span></span>
|<span data-ttu-id="e8c49-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8c49-121">Header</span></span>|<span data-ttu-id="e8c49-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e8c49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8c49-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8c49-123">Authorization</span></span>|<span data-ttu-id="e8c49-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8c49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8c49-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8c49-125">Accept</span></span>|<span data-ttu-id="e8c49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8c49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c49-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8c49-127">Request body</span></span>
<span data-ttu-id="e8c49-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8c49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8c49-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8c49-129">Response</span></span>
<span data-ttu-id="e8c49-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8c49-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8c49-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8c49-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8c49-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8c49-132">Request</span></span>
<span data-ttu-id="e8c49-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8c49-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="e8c49-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8c49-134">Response</span></span>
<span data-ttu-id="e8c49-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8c49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```



