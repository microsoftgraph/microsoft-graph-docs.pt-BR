---
title: Atualizar roleScopeTag
description: Atualize as propriedades de um objeto roleScopeTag.
ms.openlocfilehash: d18f4f47be9aab01b1221e9ce7736878bb059bed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039659"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="0332c-103">Atualizar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0332c-103">Update roleScopeTag</span></span>

> <span data-ttu-id="0332c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0332c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0332c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0332c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0332c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0332c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0332c-107">Atualize as propriedades de um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="0332c-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0332c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0332c-108">Prerequisites</span></span>
<span data-ttu-id="0332c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0332c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0332c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0332c-111">Permission type</span></span>|<span data-ttu-id="0332c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0332c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0332c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0332c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0332c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0332c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0332c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0332c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0332c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0332c-116">Not supported.</span></span>|
|<span data-ttu-id="0332c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0332c-117">Application</span></span>|<span data-ttu-id="0332c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0332c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0332c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0332c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="0332c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0332c-120">Request headers</span></span>
|<span data-ttu-id="0332c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0332c-121">Header</span></span>|<span data-ttu-id="0332c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0332c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0332c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0332c-123">Authorization</span></span>|<span data-ttu-id="0332c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0332c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0332c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0332c-125">Accept</span></span>|<span data-ttu-id="0332c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0332c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0332c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0332c-127">Request body</span></span>
<span data-ttu-id="0332c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="0332c-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="0332c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="0332c-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="0332c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0332c-130">Property</span></span>|<span data-ttu-id="0332c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0332c-131">Type</span></span>|<span data-ttu-id="0332c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0332c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0332c-133">id</span><span class="sxs-lookup"><span data-stu-id="0332c-133">id</span></span>|<span data-ttu-id="0332c-134">String</span><span class="sxs-lookup"><span data-stu-id="0332c-134">String</span></span>|<span data-ttu-id="0332c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0332c-135">Key of the entity.</span></span> <span data-ttu-id="0332c-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0332c-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0332c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0332c-137">displayName</span></span>|<span data-ttu-id="0332c-138">String</span><span class="sxs-lookup"><span data-stu-id="0332c-138">String</span></span>|<span data-ttu-id="0332c-139">A exibição ou o nome amigável da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="0332c-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0332c-140">description</span><span class="sxs-lookup"><span data-stu-id="0332c-140">description</span></span>|<span data-ttu-id="0332c-141">String</span><span class="sxs-lookup"><span data-stu-id="0332c-141">String</span></span>|<span data-ttu-id="0332c-142">Descrição da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="0332c-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="0332c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0332c-143">Response</span></span>
<span data-ttu-id="0332c-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0332c-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0332c-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0332c-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="0332c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0332c-146">Request</span></span>
<span data-ttu-id="0332c-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0332c-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="0332c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0332c-148">Response</span></span>
<span data-ttu-id="0332c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0332c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





