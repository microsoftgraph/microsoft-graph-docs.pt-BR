---
title: atribuir ação
description: Substitua todos os grupos direcionados por uma política.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa0ce371f61b13b5b987fc82fe5329305ec30e65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754329"
---
# <a name="assign-action"></a><span data-ttu-id="d08d5-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d08d5-103">assign action</span></span>

<span data-ttu-id="d08d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d08d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d08d5-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d08d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d08d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d08d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d08d5-107">Substitua todos os grupos direcionados por uma política.</span><span class="sxs-lookup"><span data-stu-id="d08d5-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d08d5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d08d5-108">Prerequisites</span></span>
<span data-ttu-id="d08d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d08d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d08d5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d08d5-111">Permission type</span></span>|<span data-ttu-id="d08d5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d08d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d08d5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d08d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d08d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d08d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d08d5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d08d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d08d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d08d5-116">Not supported.</span></span>|
|<span data-ttu-id="d08d5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d08d5-117">Application</span></span>|<span data-ttu-id="d08d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d08d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d08d5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d08d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d08d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d08d5-120">Request headers</span></span>
|<span data-ttu-id="d08d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d08d5-121">Header</span></span>|<span data-ttu-id="d08d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d08d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d08d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d08d5-123">Authorization</span></span>|<span data-ttu-id="d08d5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d08d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d08d5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d08d5-125">Accept</span></span>|<span data-ttu-id="d08d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d08d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d08d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d08d5-127">Request body</span></span>
<span data-ttu-id="d08d5-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d08d5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d08d5-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d08d5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d08d5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d08d5-130">Property</span></span>|<span data-ttu-id="d08d5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d08d5-131">Type</span></span>|<span data-ttu-id="d08d5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d08d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d08d5-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="d08d5-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="d08d5-134">[Coleção officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d08d5-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d08d5-135">Lista de atribuições de configuração do office</span><span class="sxs-lookup"><span data-stu-id="d08d5-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="d08d5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d08d5-136">Response</span></span>
<span data-ttu-id="d08d5-137">Se tiver êxito, essa ação retornará um código de resposta e uma coleção `200 OK` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d08d5-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d08d5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d08d5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d08d5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d08d5-139">Request</span></span>
<span data-ttu-id="d08d5-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d08d5-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
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

### <a name="response"></a><span data-ttu-id="d08d5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d08d5-141">Response</span></span>
<span data-ttu-id="d08d5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d08d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




