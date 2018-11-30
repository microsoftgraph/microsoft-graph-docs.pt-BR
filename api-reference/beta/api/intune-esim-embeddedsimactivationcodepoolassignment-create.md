---
title: Criar embeddedSIMActivationCodePoolAssignment
description: Crie um novo objeto de embeddedSIMActivationCodePoolAssignment.
ms.openlocfilehash: a1a4e35f72cc853d46b64033080a05ddc7d44d6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040302"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="ef0a0-103">Criar embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="ef0a0-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="ef0a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef0a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef0a0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef0a0-107">Crie um novo objeto de [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ef0a0-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef0a0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef0a0-108">Prerequisites</span></span>
<span data-ttu-id="ef0a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef0a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef0a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef0a0-111">Permission type</span></span>|<span data-ttu-id="ef0a0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef0a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef0a0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef0a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef0a0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0a0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef0a0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef0a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef0a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-116">Not supported.</span></span>|
|<span data-ttu-id="ef0a0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef0a0-117">Application</span></span>|<span data-ttu-id="ef0a0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef0a0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ef0a0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0a0-120">Request headers</span></span>
|<span data-ttu-id="ef0a0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef0a0-121">Header</span></span>|<span data-ttu-id="ef0a0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef0a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef0a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef0a0-123">Authorization</span></span>|<span data-ttu-id="ef0a0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef0a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef0a0-125">Accept</span></span>|<span data-ttu-id="ef0a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef0a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef0a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0a0-127">Request body</span></span>
<span data-ttu-id="ef0a0-128">No corpo da solicitação, fornece uma representação JSON para o objeto embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="ef0a0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o embeddedSIMActivationCodePoolAssignment.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="ef0a0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef0a0-130">Property</span></span>|<span data-ttu-id="ef0a0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef0a0-131">Type</span></span>|<span data-ttu-id="ef0a0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef0a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef0a0-133">id</span><span class="sxs-lookup"><span data-stu-id="ef0a0-133">id</span></span>|<span data-ttu-id="ef0a0-134">String</span><span class="sxs-lookup"><span data-stu-id="ef0a0-134">String</span></span>|<span data-ttu-id="ef0a0-135">Identificador exclusivo para a atribuição de pool do código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="ef0a0-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="ef0a0-137">destino</span><span class="sxs-lookup"><span data-stu-id="ef0a0-137">target</span></span>|[<span data-ttu-id="ef0a0-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ef0a0-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ef0a0-139">O tipo de grupos direcionados por pool de código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="ef0a0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0a0-140">Response</span></span>
<span data-ttu-id="ef0a0-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef0a0-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef0a0-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef0a0-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0a0-143">Request</span></span>
<span data-ttu-id="ef0a0-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ef0a0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0a0-145">Response</span></span>
<span data-ttu-id="ef0a0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef0a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





