---
title: Atualizar securityBaselineTemplate
description: Atualiza as propriedades de um objeto securityBaselineTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f2cb66df449dc8586ef3fb3f822fadf62891902
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466165"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="f8914-103">Atualizar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="f8914-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="f8914-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8914-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8914-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8914-106">Atualiza as propriedades de um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="f8914-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8914-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8914-107">Prerequisites</span></span>
<span data-ttu-id="f8914-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8914-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8914-110">Permission type</span></span>|<span data-ttu-id="f8914-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8914-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8914-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8914-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8914-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8914-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8914-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8914-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8914-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8914-115">Not supported.</span></span>|
|<span data-ttu-id="f8914-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8914-116">Application</span></span>|<span data-ttu-id="f8914-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8914-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8914-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8914-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="f8914-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8914-119">Request headers</span></span>
|<span data-ttu-id="f8914-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8914-120">Header</span></span>|<span data-ttu-id="f8914-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8914-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8914-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8914-122">Authorization</span></span>|<span data-ttu-id="f8914-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8914-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8914-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8914-124">Accept</span></span>|<span data-ttu-id="f8914-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8914-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8914-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8914-126">Request body</span></span>
<span data-ttu-id="f8914-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="f8914-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="f8914-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f8914-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="f8914-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8914-129">Property</span></span>|<span data-ttu-id="f8914-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8914-130">Type</span></span>|<span data-ttu-id="f8914-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8914-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8914-132">id</span><span class="sxs-lookup"><span data-stu-id="f8914-132">id</span></span>|<span data-ttu-id="f8914-133">String</span><span class="sxs-lookup"><span data-stu-id="f8914-133">String</span></span>|<span data-ttu-id="f8914-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f8914-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="f8914-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f8914-135">displayName</span></span>|<span data-ttu-id="f8914-136">String</span><span class="sxs-lookup"><span data-stu-id="f8914-136">String</span></span>|<span data-ttu-id="f8914-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f8914-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="f8914-138">description</span><span class="sxs-lookup"><span data-stu-id="f8914-138">description</span></span>|<span data-ttu-id="f8914-139">String</span><span class="sxs-lookup"><span data-stu-id="f8914-139">String</span></span>|<span data-ttu-id="f8914-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f8914-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f8914-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8914-141">Response</span></span>
<span data-ttu-id="f8914-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8914-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8914-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8914-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8914-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8914-144">Request</span></span>
<span data-ttu-id="f8914-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8914-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f8914-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8914-146">Response</span></span>
<span data-ttu-id="f8914-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8914-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





