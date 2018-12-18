---
title: atribuir ação
description: Substitua direcionados todos os grupos de uma política.
author: tfitzmac
ms.openlocfilehash: 00ecb5d5e34fb067bbca36eee5ff190344319d7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307823"
---
# <a name="assign-action"></a><span data-ttu-id="59193-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="59193-103">assign action</span></span>

> <span data-ttu-id="59193-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="59193-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59193-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="59193-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59193-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="59193-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59193-107">Substitua direcionados todos os grupos de uma política.</span><span class="sxs-lookup"><span data-stu-id="59193-107">Replace all targeted groups for a policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59193-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59193-108">Prerequisites</span></span>
<span data-ttu-id="59193-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59193-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59193-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59193-111">Permission type</span></span>|<span data-ttu-id="59193-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59193-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59193-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59193-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59193-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59193-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59193-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59193-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59193-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59193-116">Not supported.</span></span>|
|<span data-ttu-id="59193-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59193-117">Application</span></span>|<span data-ttu-id="59193-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59193-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59193-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59193-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="59193-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59193-120">Request headers</span></span>
|<span data-ttu-id="59193-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59193-121">Header</span></span>|<span data-ttu-id="59193-122">Valor</span><span class="sxs-lookup"><span data-stu-id="59193-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59193-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59193-123">Authorization</span></span>|<span data-ttu-id="59193-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59193-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59193-125">Accept</span><span class="sxs-lookup"><span data-stu-id="59193-125">Accept</span></span>|<span data-ttu-id="59193-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59193-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59193-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59193-127">Request body</span></span>
<span data-ttu-id="59193-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="59193-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="59193-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="59193-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="59193-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59193-130">Property</span></span>|<span data-ttu-id="59193-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="59193-131">Type</span></span>|<span data-ttu-id="59193-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="59193-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59193-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="59193-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="59193-134">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="59193-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="59193-135">Lista de atribuições de configuração do office</span><span class="sxs-lookup"><span data-stu-id="59193-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="59193-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="59193-136">Response</span></span>
<span data-ttu-id="59193-137">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um conjunto de [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59193-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59193-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59193-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="59193-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59193-139">Request</span></span>
<span data-ttu-id="59193-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59193-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59193-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="59193-141">Response</span></span>
<span data-ttu-id="59193-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59193-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



