---
title: Criar roleScopeTag
description: Crie um novo objeto de roleScopeTag.
ms.openlocfilehash: b2f42999c785786175e5a6fb4dfd2b510d148927
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036677"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="2b4da-103">Criar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2b4da-103">Create roleScopeTag</span></span>

> <span data-ttu-id="2b4da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b4da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b4da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b4da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b4da-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b4da-107">Crie um novo objeto de [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="2b4da-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b4da-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b4da-108">Prerequisites</span></span>
<span data-ttu-id="2b4da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b4da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b4da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b4da-111">Permission type</span></span>|<span data-ttu-id="2b4da-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b4da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b4da-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b4da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b4da-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b4da-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2b4da-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b4da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b4da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b4da-116">Not supported.</span></span>|
|<span data-ttu-id="2b4da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b4da-117">Application</span></span>|<span data-ttu-id="2b4da-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b4da-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b4da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b4da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="2b4da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b4da-120">Request headers</span></span>
|<span data-ttu-id="2b4da-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b4da-121">Header</span></span>|<span data-ttu-id="2b4da-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b4da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b4da-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b4da-123">Authorization</span></span>|<span data-ttu-id="2b4da-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b4da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b4da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b4da-125">Accept</span></span>|<span data-ttu-id="2b4da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b4da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b4da-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b4da-127">Request body</span></span>
<span data-ttu-id="2b4da-128">No corpo da solicitação, fornece uma representação JSON para o objeto roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="2b4da-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="2b4da-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="2b4da-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="2b4da-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b4da-130">Property</span></span>|<span data-ttu-id="2b4da-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b4da-131">Type</span></span>|<span data-ttu-id="2b4da-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b4da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b4da-133">id</span><span class="sxs-lookup"><span data-stu-id="2b4da-133">id</span></span>|<span data-ttu-id="2b4da-134">String</span><span class="sxs-lookup"><span data-stu-id="2b4da-134">String</span></span>|<span data-ttu-id="2b4da-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2b4da-135">Key of the entity.</span></span> <span data-ttu-id="2b4da-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2b4da-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2b4da-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2b4da-137">displayName</span></span>|<span data-ttu-id="2b4da-138">String</span><span class="sxs-lookup"><span data-stu-id="2b4da-138">String</span></span>|<span data-ttu-id="2b4da-139">A exibição ou o nome amigável da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="2b4da-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="2b4da-140">description</span><span class="sxs-lookup"><span data-stu-id="2b4da-140">description</span></span>|<span data-ttu-id="2b4da-141">String</span><span class="sxs-lookup"><span data-stu-id="2b4da-141">String</span></span>|<span data-ttu-id="2b4da-142">Descrição da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="2b4da-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="2b4da-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b4da-143">Response</span></span>
<span data-ttu-id="2b4da-144">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b4da-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b4da-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b4da-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b4da-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b4da-146">Request</span></span>
<span data-ttu-id="2b4da-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b4da-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="2b4da-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b4da-148">Response</span></span>
<span data-ttu-id="2b4da-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b4da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





