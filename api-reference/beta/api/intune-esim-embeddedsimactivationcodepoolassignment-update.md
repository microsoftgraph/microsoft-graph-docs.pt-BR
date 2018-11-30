---
title: Atualizar embeddedSIMActivationCodePoolAssignment
description: Atualize as propriedades de um objeto embeddedSIMActivationCodePoolAssignment.
ms.openlocfilehash: 0a158496ea67c4b6feb7c291d4065ccd5f6d1ce9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037451"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="26118-103">Atualizar embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="26118-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="26118-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26118-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26118-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26118-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26118-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="26118-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26118-107">Atualize as propriedades de um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="26118-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26118-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26118-108">Prerequisites</span></span>
<span data-ttu-id="26118-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26118-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26118-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26118-111">Permission type</span></span>|<span data-ttu-id="26118-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26118-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26118-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26118-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26118-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26118-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26118-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26118-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26118-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26118-116">Not supported.</span></span>|
|<span data-ttu-id="26118-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26118-117">Application</span></span>|<span data-ttu-id="26118-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26118-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26118-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26118-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="26118-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26118-120">Request headers</span></span>
|<span data-ttu-id="26118-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26118-121">Header</span></span>|<span data-ttu-id="26118-122">Valor</span><span class="sxs-lookup"><span data-stu-id="26118-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26118-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26118-123">Authorization</span></span>|<span data-ttu-id="26118-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26118-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26118-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26118-125">Accept</span></span>|<span data-ttu-id="26118-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26118-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26118-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26118-127">Request body</span></span>
<span data-ttu-id="26118-128">No corpo da solicitação, fornece uma representação JSON para o objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="26118-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="26118-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26118-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="26118-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26118-130">Property</span></span>|<span data-ttu-id="26118-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26118-131">Type</span></span>|<span data-ttu-id="26118-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26118-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26118-133">id</span><span class="sxs-lookup"><span data-stu-id="26118-133">id</span></span>|<span data-ttu-id="26118-134">String</span><span class="sxs-lookup"><span data-stu-id="26118-134">String</span></span>|<span data-ttu-id="26118-135">Identificador exclusivo para a atribuição de pool do código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="26118-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="26118-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="26118-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="26118-137">destino</span><span class="sxs-lookup"><span data-stu-id="26118-137">target</span></span>|[<span data-ttu-id="26118-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="26118-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="26118-139">O tipo de grupos direcionados por pool de código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="26118-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="26118-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="26118-140">Response</span></span>
<span data-ttu-id="26118-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26118-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26118-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26118-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="26118-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26118-143">Request</span></span>
<span data-ttu-id="26118-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26118-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="26118-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="26118-145">Response</span></span>
<span data-ttu-id="26118-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26118-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





