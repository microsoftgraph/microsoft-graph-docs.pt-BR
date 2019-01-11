---
title: Atualizar roleScopeTag
description: Atualize as propriedades de um objeto roleScopeTag.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bece75c05fa65a2c5def34ec1644a7375711ab97
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808131"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="02881-103">Atualizar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="02881-103">Update roleScopeTag</span></span>

> <span data-ttu-id="02881-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="02881-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02881-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="02881-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02881-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="02881-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02881-107">Atualize as propriedades de um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="02881-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02881-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02881-108">Prerequisites</span></span>
<span data-ttu-id="02881-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02881-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02881-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02881-111">Permission type</span></span>|<span data-ttu-id="02881-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02881-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02881-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02881-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02881-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02881-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="02881-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02881-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02881-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02881-116">Not supported.</span></span>|
|<span data-ttu-id="02881-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02881-117">Application</span></span>|<span data-ttu-id="02881-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02881-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02881-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02881-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="02881-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02881-120">Request headers</span></span>
|<span data-ttu-id="02881-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02881-121">Header</span></span>|<span data-ttu-id="02881-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02881-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02881-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02881-123">Authorization</span></span>|<span data-ttu-id="02881-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02881-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02881-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02881-125">Accept</span></span>|<span data-ttu-id="02881-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02881-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02881-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02881-127">Request body</span></span>
<span data-ttu-id="02881-128">No corpo da solicitação, fornece uma representação JSON para o objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="02881-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="02881-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="02881-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="02881-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02881-130">Property</span></span>|<span data-ttu-id="02881-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02881-131">Type</span></span>|<span data-ttu-id="02881-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02881-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02881-133">id</span><span class="sxs-lookup"><span data-stu-id="02881-133">id</span></span>|<span data-ttu-id="02881-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02881-134">String</span></span>|<span data-ttu-id="02881-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02881-135">Key of the entity.</span></span> <span data-ttu-id="02881-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="02881-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="02881-137">displayName</span><span class="sxs-lookup"><span data-stu-id="02881-137">displayName</span></span>|<span data-ttu-id="02881-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02881-138">String</span></span>|<span data-ttu-id="02881-139">A exibição ou o nome amigável da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="02881-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="02881-140">description</span><span class="sxs-lookup"><span data-stu-id="02881-140">description</span></span>|<span data-ttu-id="02881-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02881-141">String</span></span>|<span data-ttu-id="02881-142">Descrição da marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="02881-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="02881-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="02881-143">Response</span></span>
<span data-ttu-id="02881-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02881-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02881-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02881-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="02881-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02881-146">Request</span></span>
<span data-ttu-id="02881-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02881-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="02881-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="02881-148">Response</span></span>
<span data-ttu-id="02881-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02881-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





