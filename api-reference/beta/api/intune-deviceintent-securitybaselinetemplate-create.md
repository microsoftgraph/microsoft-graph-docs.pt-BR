---
title: Criar securityBaselineTemplate
description: Criar um novo objeto securityBaselineTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95222dba49c3cdcb807f610c67bcd94081d9bfe6
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522836"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="eb204-103">Criar securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="eb204-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="eb204-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb204-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb204-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb204-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb204-106">Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="eb204-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb204-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb204-107">Prerequisites</span></span>
<span data-ttu-id="eb204-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb204-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb204-110">Permission type</span></span>|<span data-ttu-id="eb204-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb204-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb204-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb204-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb204-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb204-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb204-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb204-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb204-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb204-115">Not supported.</span></span>|
|<span data-ttu-id="eb204-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb204-116">Application</span></span>|<span data-ttu-id="eb204-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb204-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb204-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb204-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
```

## <a name="request-headers"></a><span data-ttu-id="eb204-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb204-119">Request headers</span></span>
|<span data-ttu-id="eb204-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb204-120">Header</span></span>|<span data-ttu-id="eb204-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb204-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb204-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb204-122">Authorization</span></span>|<span data-ttu-id="eb204-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb204-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb204-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb204-124">Accept</span></span>|<span data-ttu-id="eb204-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb204-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb204-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb204-126">Request body</span></span>
<span data-ttu-id="eb204-127">No corpo da solicitação, forneça uma representação JSON do objeto securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="eb204-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="eb204-128">A tabela a seguir mostra as propriedades que são necessárias ao criar securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="eb204-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="eb204-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb204-129">Property</span></span>|<span data-ttu-id="eb204-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb204-130">Type</span></span>|<span data-ttu-id="eb204-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb204-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb204-132">id</span><span class="sxs-lookup"><span data-stu-id="eb204-132">id</span></span>|<span data-ttu-id="eb204-133">String</span><span class="sxs-lookup"><span data-stu-id="eb204-133">String</span></span>|<span data-ttu-id="eb204-134">A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="eb204-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="eb204-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eb204-135">displayName</span></span>|<span data-ttu-id="eb204-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="eb204-136">String</span></span>|<span data-ttu-id="eb204-137">O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="eb204-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="eb204-138">description</span><span class="sxs-lookup"><span data-stu-id="eb204-138">description</span></span>|<span data-ttu-id="eb204-139">String</span><span class="sxs-lookup"><span data-stu-id="eb204-139">String</span></span>|<span data-ttu-id="eb204-140">A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="eb204-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="eb204-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb204-141">Response</span></span>
<span data-ttu-id="eb204-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb204-142">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb204-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb204-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb204-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb204-144">Request</span></span>
<span data-ttu-id="eb204-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb204-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="eb204-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb204-146">Response</span></span>
<span data-ttu-id="eb204-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb204-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```







