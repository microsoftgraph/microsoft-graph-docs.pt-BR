---
title: Listar officeClientConfigurationAssignments
description: Listar propriedades e relações dos objetos officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 570281f3961f1f4449ae9050cd77b12863452fc3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665641"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="24491-103">Listar officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="24491-103">List officeClientConfigurationAssignments</span></span>

<span data-ttu-id="24491-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24491-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24491-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24491-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24491-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24491-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24491-107">Listar propriedades e relações dos [objetos officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="24491-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24491-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24491-108">Prerequisites</span></span>
<span data-ttu-id="24491-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24491-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24491-111">Permission type</span></span>|<span data-ttu-id="24491-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24491-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24491-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24491-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24491-114">\*\*TODO: Determinar escopos \*\*</span><span class="sxs-lookup"><span data-stu-id="24491-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="24491-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24491-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24491-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24491-116">Not supported.</span></span>|
|<span data-ttu-id="24491-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24491-117">Application</span></span>|<span data-ttu-id="24491-118">\*\*TODO: Determinar escopos \*\*</span><span class="sxs-lookup"><span data-stu-id="24491-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="24491-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24491-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="24491-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24491-120">Request headers</span></span>
|<span data-ttu-id="24491-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24491-121">Header</span></span>|<span data-ttu-id="24491-122">Valor</span><span class="sxs-lookup"><span data-stu-id="24491-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24491-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24491-123">Authorization</span></span>|<span data-ttu-id="24491-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24491-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24491-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24491-125">Accept</span></span>|<span data-ttu-id="24491-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24491-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24491-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24491-127">Request body</span></span>
<span data-ttu-id="24491-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24491-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24491-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="24491-129">Response</span></span>
<span data-ttu-id="24491-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24491-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24491-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24491-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24491-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24491-132">Request</span></span>
<span data-ttu-id="24491-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24491-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="24491-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="24491-134">Response</span></span>
<span data-ttu-id="24491-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24491-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




