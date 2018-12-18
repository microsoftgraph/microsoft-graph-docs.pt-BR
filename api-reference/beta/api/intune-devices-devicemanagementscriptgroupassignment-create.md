---
title: Criar deviceManagementScriptGroupAssignment
description: Crie um novo objeto de deviceManagementScriptGroupAssignment.
author: tfitzmac
ms.openlocfilehash: f084fb933d4694d9c1dfa43f018fb3ce2d8dd95b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324777"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="549e7-103">Criar deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="549e7-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="549e7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="549e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="549e7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="549e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="549e7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="549e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="549e7-107">Crie um novo objeto de [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="549e7-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="549e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="549e7-108">Prerequisites</span></span>
<span data-ttu-id="549e7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="549e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="549e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="549e7-111">Permission type</span></span>|<span data-ttu-id="549e7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="549e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="549e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="549e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="549e7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="549e7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="549e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="549e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="549e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="549e7-116">Not supported.</span></span>|
|<span data-ttu-id="549e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="549e7-117">Application</span></span>|<span data-ttu-id="549e7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="549e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="549e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="549e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="549e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="549e7-120">Request headers</span></span>
|<span data-ttu-id="549e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="549e7-121">Header</span></span>|<span data-ttu-id="549e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="549e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="549e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="549e7-123">Authorization</span></span>|<span data-ttu-id="549e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="549e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="549e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="549e7-125">Accept</span></span>|<span data-ttu-id="549e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="549e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="549e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="549e7-127">Request body</span></span>
<span data-ttu-id="549e7-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="549e7-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="549e7-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceManagementScriptGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="549e7-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="549e7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="549e7-130">Property</span></span>|<span data-ttu-id="549e7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="549e7-131">Type</span></span>|<span data-ttu-id="549e7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="549e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="549e7-133">id</span><span class="sxs-lookup"><span data-stu-id="549e7-133">id</span></span>|<span data-ttu-id="549e7-134">String</span><span class="sxs-lookup"><span data-stu-id="549e7-134">String</span></span>|<span data-ttu-id="549e7-135">Chave da entidade de atribuição de grupo de script para gerenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="549e7-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="549e7-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="549e7-136">targetGroupId</span></span>|<span data-ttu-id="549e7-137">String</span><span class="sxs-lookup"><span data-stu-id="549e7-137">String</span></span>|<span data-ttu-id="549e7-138">A Id de grupo do Active Directory do Windows Azure Pretendemos o script.</span><span class="sxs-lookup"><span data-stu-id="549e7-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="549e7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="549e7-139">Response</span></span>
<span data-ttu-id="549e7-140">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="549e7-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="549e7-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="549e7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="549e7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="549e7-142">Request</span></span>
<span data-ttu-id="549e7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="549e7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="549e7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="549e7-144">Response</span></span>
<span data-ttu-id="549e7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="549e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





