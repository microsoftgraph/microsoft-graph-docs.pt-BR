---
title: Criar roleScopeTag
description: Crie um novo objeto de roleScopeTag.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 205269e93ba0f24afc37ef64d4c2ed0da1036ca1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827437"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="3e5cc-103">Criar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3e5cc-103">Create roleScopeTag</span></span>

> <span data-ttu-id="3e5cc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e5cc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e5cc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e5cc-107">Crie um novo objeto de [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="3e5cc-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e5cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e5cc-108">Prerequisites</span></span>
<span data-ttu-id="3e5cc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e5cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e5cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e5cc-111">Permission type</span></span>|<span data-ttu-id="3e5cc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e5cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e5cc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e5cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e5cc-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e5cc-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3e5cc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e5cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e5cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-116">Not supported.</span></span>|
|<span data-ttu-id="3e5cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e5cc-117">Application</span></span>|<span data-ttu-id="3e5cc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e5cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e5cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="3e5cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e5cc-120">Request headers</span></span>
|<span data-ttu-id="3e5cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e5cc-121">Header</span></span>|<span data-ttu-id="3e5cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3e5cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e5cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e5cc-123">Authorization</span></span>|<span data-ttu-id="3e5cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e5cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e5cc-125">Accept</span></span>|<span data-ttu-id="3e5cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e5cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e5cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e5cc-127">Request body</span></span>
<span data-ttu-id="3e5cc-128">No corpo da solicitação, fornece uma representação JSON para o objeto roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="3e5cc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="3e5cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e5cc-130">Property</span></span>|<span data-ttu-id="3e5cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e5cc-131">Type</span></span>|<span data-ttu-id="3e5cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e5cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e5cc-133">id</span><span class="sxs-lookup"><span data-stu-id="3e5cc-133">id</span></span>|<span data-ttu-id="3e5cc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e5cc-134">String</span></span>|<span data-ttu-id="3e5cc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-135">Key of the entity.</span></span> <span data-ttu-id="3e5cc-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3e5cc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3e5cc-137">displayName</span></span>|<span data-ttu-id="3e5cc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e5cc-138">String</span></span>|<span data-ttu-id="3e5cc-139">A exibição ou o nome amigável da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="3e5cc-140">description</span><span class="sxs-lookup"><span data-stu-id="3e5cc-140">description</span></span>|<span data-ttu-id="3e5cc-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e5cc-141">String</span></span>|<span data-ttu-id="3e5cc-142">Descrição da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="3e5cc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e5cc-143">Response</span></span>
<span data-ttu-id="3e5cc-144">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e5cc-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e5cc-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e5cc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e5cc-146">Request</span></span>
<span data-ttu-id="3e5cc-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e5cc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e5cc-148">Response</span></span>
<span data-ttu-id="3e5cc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e5cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





