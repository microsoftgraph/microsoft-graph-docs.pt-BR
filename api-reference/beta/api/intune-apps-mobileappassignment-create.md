---
title: Criar mobileAppAssignment
description: Criar um novo objeto mobileAppAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 94fb6e79077e687df11cda4b28b71b8e97360971
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397978"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="bff5f-103">Criar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bff5f-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="bff5f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bff5f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bff5f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bff5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bff5f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bff5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bff5f-107">Criar um novo objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bff5f-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bff5f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bff5f-108">Prerequisites</span></span>
<span data-ttu-id="bff5f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bff5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bff5f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bff5f-111">Permission type</span></span>|<span data-ttu-id="bff5f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bff5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bff5f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bff5f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bff5f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff5f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bff5f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bff5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bff5f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bff5f-116">Not supported.</span></span>|
|<span data-ttu-id="bff5f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bff5f-117">Application</span></span>|<span data-ttu-id="bff5f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bff5f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bff5f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bff5f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bff5f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bff5f-120">Request headers</span></span>
|<span data-ttu-id="bff5f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bff5f-121">Header</span></span>|<span data-ttu-id="bff5f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bff5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bff5f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bff5f-123">Authorization</span></span>|<span data-ttu-id="bff5f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bff5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bff5f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bff5f-125">Accept</span></span>|<span data-ttu-id="bff5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bff5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bff5f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bff5f-127">Request body</span></span>
<span data-ttu-id="bff5f-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="bff5f-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="bff5f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="bff5f-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="bff5f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bff5f-130">Property</span></span>|<span data-ttu-id="bff5f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bff5f-131">Type</span></span>|<span data-ttu-id="bff5f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bff5f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bff5f-133">id</span><span class="sxs-lookup"><span data-stu-id="bff5f-133">id</span></span>|<span data-ttu-id="bff5f-134">String</span><span class="sxs-lookup"><span data-stu-id="bff5f-134">String</span></span>|<span data-ttu-id="bff5f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bff5f-135">Key of the entity.</span></span>|
|<span data-ttu-id="bff5f-136">finalidade</span><span class="sxs-lookup"><span data-stu-id="bff5f-136">intent</span></span>|[<span data-ttu-id="bff5f-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="bff5f-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="bff5f-138">A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="bff5f-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="bff5f-139">destino</span><span class="sxs-lookup"><span data-stu-id="bff5f-139">target</span></span>|[<span data-ttu-id="bff5f-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bff5f-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bff5f-141">A atribuição do grupo de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bff5f-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="bff5f-142">configurações</span><span class="sxs-lookup"><span data-stu-id="bff5f-142">settings</span></span>|[<span data-ttu-id="bff5f-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="bff5f-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="bff5f-144">As configurações para a atribuição de destino definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bff5f-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="bff5f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bff5f-145">Response</span></span>
<span data-ttu-id="bff5f-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bff5f-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bff5f-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bff5f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="bff5f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bff5f-148">Request</span></span>
<span data-ttu-id="bff5f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bff5f-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bff5f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bff5f-150">Response</span></span>
<span data-ttu-id="bff5f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bff5f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




