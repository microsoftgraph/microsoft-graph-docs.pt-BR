---
title: Listar officeClientConfigurationAssignments
description: Listar Propriedades e relações dos objetos officeClientConfigurationAssignment.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 074118e023750199f6d4a1f824c920aac7e0edd2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930454"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="ba1ae-103">Listar officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="ba1ae-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="ba1ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1ae-106">Listar Propriedades e relações dos objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ba1ae-106">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba1ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba1ae-107">Prerequisites</span></span>
<span data-ttu-id="ba1ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba1ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba1ae-110">Permission type</span></span>|<span data-ttu-id="ba1ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba1ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba1ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba1ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba1ae-113">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="ba1ae-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="ba1ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba1ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba1ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-115">Not supported.</span></span>|
|<span data-ttu-id="ba1ae-116">Application</span><span class="sxs-lookup"><span data-stu-id="ba1ae-116">Application</span></span>|<span data-ttu-id="ba1ae-117">\* \* TODO: determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="ba1ae-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba1ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba1ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ba1ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1ae-119">Request headers</span></span>
|<span data-ttu-id="ba1ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba1ae-120">Header</span></span>|<span data-ttu-id="ba1ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ba1ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba1ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba1ae-122">Authorization</span></span>|<span data-ttu-id="ba1ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba1ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba1ae-124">Accept</span></span>|<span data-ttu-id="ba1ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba1ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1ae-126">Request body</span></span>
<span data-ttu-id="ba1ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba1ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1ae-128">Response</span></span>
<span data-ttu-id="ba1ae-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba1ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba1ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba1ae-131">Request</span></span>
<span data-ttu-id="ba1ae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="ba1ae-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba1ae-133">Response</span></span>
<span data-ttu-id="ba1ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba1ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





