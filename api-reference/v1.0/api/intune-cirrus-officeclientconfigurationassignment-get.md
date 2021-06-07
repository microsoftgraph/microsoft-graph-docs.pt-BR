---
title: Obter officeClientConfigurationAssignment
description: Leia propriedades e relações do objeto officeClientConfigurationAssignment.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82380a555c0dade29463b78297ddde0cc96348f0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752930"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="56bf8-103">Obter officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="56bf8-103">Get officeClientConfigurationAssignment</span></span>

<span data-ttu-id="56bf8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56bf8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56bf8-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56bf8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56bf8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56bf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56bf8-107">Leia propriedades e relações do [objeto officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="56bf8-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56bf8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56bf8-108">Prerequisites</span></span>
<span data-ttu-id="56bf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56bf8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56bf8-111">Permission type</span></span>|<span data-ttu-id="56bf8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56bf8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56bf8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56bf8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56bf8-114">\*\*TODO: Determinar escopos \*\*</span><span class="sxs-lookup"><span data-stu-id="56bf8-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="56bf8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56bf8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56bf8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56bf8-116">Not supported.</span></span>|
|<span data-ttu-id="56bf8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56bf8-117">Application</span></span>|<span data-ttu-id="56bf8-118">\*\*TODO: Determinar escopos \*\*</span><span class="sxs-lookup"><span data-stu-id="56bf8-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="56bf8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56bf8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56bf8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56bf8-120">Optional query parameters</span></span>
<span data-ttu-id="56bf8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56bf8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56bf8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56bf8-122">Request headers</span></span>
|<span data-ttu-id="56bf8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56bf8-123">Header</span></span>|<span data-ttu-id="56bf8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="56bf8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56bf8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="56bf8-125">Authorization</span></span>|<span data-ttu-id="56bf8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56bf8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56bf8-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56bf8-127">Accept</span></span>|<span data-ttu-id="56bf8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="56bf8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56bf8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56bf8-129">Request body</span></span>
<span data-ttu-id="56bf8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56bf8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56bf8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="56bf8-131">Response</span></span>
<span data-ttu-id="56bf8-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56bf8-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56bf8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56bf8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="56bf8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56bf8-134">Request</span></span>
<span data-ttu-id="56bf8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56bf8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="56bf8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="56bf8-136">Response</span></span>
<span data-ttu-id="56bf8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56bf8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```




