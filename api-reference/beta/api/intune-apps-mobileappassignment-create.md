---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8ceae2f0bacac3d83532a6aa9b338c32573d6332
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874652"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="96fb7-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="96fb7-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="96fb7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96fb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96fb7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96fb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96fb7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96fb7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96fb7-107">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="96fb7-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96fb7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96fb7-108">Prerequisites</span></span>
<span data-ttu-id="96fb7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96fb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96fb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96fb7-111">Permission type</span></span>|<span data-ttu-id="96fb7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96fb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96fb7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96fb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96fb7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96fb7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96fb7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96fb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96fb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96fb7-116">Not supported.</span></span>|
|<span data-ttu-id="96fb7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96fb7-117">Application</span></span>|<span data-ttu-id="96fb7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96fb7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96fb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96fb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="96fb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96fb7-120">Request headers</span></span>
|<span data-ttu-id="96fb7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96fb7-121">Header</span></span>|<span data-ttu-id="96fb7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96fb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96fb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96fb7-123">Authorization</span></span>|<span data-ttu-id="96fb7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96fb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96fb7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96fb7-125">Accept</span></span>|<span data-ttu-id="96fb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96fb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96fb7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96fb7-127">Request body</span></span>
<span data-ttu-id="96fb7-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="96fb7-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="96fb7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="96fb7-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="96fb7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96fb7-130">Property</span></span>|<span data-ttu-id="96fb7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="96fb7-131">Type</span></span>|<span data-ttu-id="96fb7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="96fb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96fb7-133">id</span><span class="sxs-lookup"><span data-stu-id="96fb7-133">id</span></span>|<span data-ttu-id="96fb7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96fb7-134">String</span></span>|<span data-ttu-id="96fb7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96fb7-135">Key of the entity.</span></span>|
|<span data-ttu-id="96fb7-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="96fb7-136">intent</span></span>|[<span data-ttu-id="96fb7-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="96fb7-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="96fb7-138">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="96fb7-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="96fb7-139">destino</span><span class="sxs-lookup"><span data-stu-id="96fb7-139">target</span></span>|[<span data-ttu-id="96fb7-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="96fb7-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="96fb7-141">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="96fb7-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="96fb7-142">configurações</span><span class="sxs-lookup"><span data-stu-id="96fb7-142">settings</span></span>|[<span data-ttu-id="96fb7-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="96fb7-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="96fb7-144">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="96fb7-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="96fb7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="96fb7-145">Response</span></span>
<span data-ttu-id="96fb7-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96fb7-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96fb7-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96fb7-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="96fb7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96fb7-148">Request</span></span>
<span data-ttu-id="96fb7-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96fb7-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="96fb7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="96fb7-150">Response</span></span>
<span data-ttu-id="96fb7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96fb7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```





