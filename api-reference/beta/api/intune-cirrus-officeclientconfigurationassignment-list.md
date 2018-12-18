---
title: Lista officeClientConfigurationAssignments
description: Lista as propriedades e os relacionamentos dos objetos officeClientConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 34f926b0e02a963c1ab16ec7a0dd3eefcc06852c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360379"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="ddbef-103">Lista officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="ddbef-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="ddbef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddbef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddbef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddbef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddbef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ddbef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddbef-107">Lista as propriedades e os relacionamentos dos objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ddbef-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddbef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddbef-108">Prerequisites</span></span>
<span data-ttu-id="ddbef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddbef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddbef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddbef-111">Permission type</span></span>|<span data-ttu-id="ddbef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddbef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddbef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddbef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddbef-114">\* \* TODO: Determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="ddbef-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="ddbef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddbef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddbef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddbef-116">Not supported.</span></span>|
|<span data-ttu-id="ddbef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddbef-117">Application</span></span>|<span data-ttu-id="ddbef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddbef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddbef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddbef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ddbef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddbef-120">Request headers</span></span>
|<span data-ttu-id="ddbef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddbef-121">Header</span></span>|<span data-ttu-id="ddbef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ddbef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddbef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddbef-123">Authorization</span></span>|<span data-ttu-id="ddbef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddbef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddbef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddbef-125">Accept</span></span>|<span data-ttu-id="ddbef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddbef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddbef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddbef-127">Request body</span></span>
<span data-ttu-id="ddbef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddbef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddbef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddbef-129">Response</span></span>
<span data-ttu-id="ddbef-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddbef-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddbef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddbef-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddbef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddbef-132">Request</span></span>
<span data-ttu-id="ddbef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddbef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="ddbef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddbef-134">Response</span></span>
<span data-ttu-id="ddbef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddbef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



