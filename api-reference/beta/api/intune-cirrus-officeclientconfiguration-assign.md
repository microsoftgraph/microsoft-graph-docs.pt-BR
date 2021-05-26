---
title: Office configuração do cliente atribuir ação
description: Substitua todos os grupos direcionados por uma política.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4fb8f6d2bb05e5809337ed4be0010f8f6cb470f4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665652"
---
# <a name="office-client-configuration-assign--assign-action"></a><span data-ttu-id="f822f-103">Office configuração do cliente atribuir ação de atribuição</span><span class="sxs-lookup"><span data-stu-id="f822f-103">Office client configuration assign  assign action</span></span>

<span data-ttu-id="f822f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f822f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f822f-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f822f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f822f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f822f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f822f-107">Substitua todos os grupos direcionados por uma política.</span><span class="sxs-lookup"><span data-stu-id="f822f-107">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f822f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f822f-108">Prerequisites</span></span>
<span data-ttu-id="f822f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f822f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f822f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f822f-111">Permission type</span></span>|<span data-ttu-id="f822f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f822f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f822f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f822f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f822f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f822f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f822f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f822f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f822f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f822f-116">Not supported.</span></span>|
|<span data-ttu-id="f822f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f822f-117">Application</span></span>|<span data-ttu-id="f822f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f822f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f822f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f822f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f822f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f822f-120">Request headers</span></span>
|<span data-ttu-id="f822f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f822f-121">Header</span></span>|<span data-ttu-id="f822f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f822f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f822f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f822f-123">Authorization</span></span>|<span data-ttu-id="f822f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f822f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f822f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f822f-125">Accept</span></span>|<span data-ttu-id="f822f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f822f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f822f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f822f-127">Request body</span></span>
<span data-ttu-id="f822f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f822f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f822f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f822f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f822f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f822f-130">Property</span></span>|<span data-ttu-id="f822f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f822f-131">Type</span></span>|<span data-ttu-id="f822f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f822f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f822f-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="f822f-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="f822f-134">[Coleção officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f822f-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f822f-135">Lista de atribuições de configuração do office</span><span class="sxs-lookup"><span data-stu-id="f822f-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="f822f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f822f-136">Response</span></span>
<span data-ttu-id="f822f-137">Se tiver êxito, essa ação retornará um código de resposta e uma coleção `200 OK` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f822f-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f822f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f822f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f822f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f822f-139">Request</span></span>
<span data-ttu-id="f822f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f822f-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f822f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f822f-141">Response</span></span>
<span data-ttu-id="f822f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f822f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




