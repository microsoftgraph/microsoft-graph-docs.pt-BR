---
title: Atualizar officeClientConfigurationAssignment
description: Atualize as propriedades de um objeto officeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f3d2fab5dc8793f566973e2d3e2d9bf968cbf30a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817525"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="d4c5c-103">Atualizar officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d4c5c-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="d4c5c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4c5c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4c5c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4c5c-107">Atualize as propriedades de um objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c5c-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4c5c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4c5c-108">Prerequisites</span></span>
<span data-ttu-id="d4c5c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c5c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4c5c-111">Permission type</span></span>|<span data-ttu-id="d4c5c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4c5c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c5c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4c5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c5c-114">\* \* TODO: Determinar escopos \* \*</span><span class="sxs-lookup"><span data-stu-id="d4c5c-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="d4c5c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4c5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-116">Not supported.</span></span>|
|<span data-ttu-id="d4c5c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4c5c-117">Application</span></span>|<span data-ttu-id="d4c5c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4c5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d4c5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c5c-120">Request headers</span></span>
|<span data-ttu-id="d4c5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4c5c-121">Header</span></span>|<span data-ttu-id="d4c5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4c5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4c5c-123">Authorization</span></span>|<span data-ttu-id="d4c5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4c5c-125">Accept</span></span>|<span data-ttu-id="d4c5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c5c-127">Request body</span></span>
<span data-ttu-id="d4c5c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c5c-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="d4c5c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d4c5c-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="d4c5c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4c5c-130">Property</span></span>|<span data-ttu-id="d4c5c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4c5c-131">Type</span></span>|<span data-ttu-id="d4c5c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4c5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c5c-133">id</span><span class="sxs-lookup"><span data-stu-id="d4c5c-133">id</span></span>|<span data-ttu-id="d4c5c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4c5c-134">String</span></span>|<span data-ttu-id="d4c5c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d4c5c-135">Not yet documented</span></span>|
|<span data-ttu-id="d4c5c-136">destino</span><span class="sxs-lookup"><span data-stu-id="d4c5c-136">target</span></span>|[<span data-ttu-id="d4c5c-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d4c5c-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="d4c5c-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d4c5c-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d4c5c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4c5c-139">Response</span></span>
<span data-ttu-id="d4c5c-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c5c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4c5c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4c5c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c5c-142">Request</span></span>
<span data-ttu-id="d4c5c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d4c5c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4c5c-144">Response</span></span>
<span data-ttu-id="d4c5c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



