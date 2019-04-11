---
title: Criar deviceManagementTemplate
description: Criar um novo objeto deviceManagementTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23c86d654d229c4932a9e5b7d86d980416637b2a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807921"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="2138e-103">Criar deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="2138e-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="2138e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2138e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2138e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2138e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2138e-106">Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="2138e-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2138e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2138e-107">Prerequisites</span></span>
<span data-ttu-id="2138e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2138e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2138e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2138e-110">Permission type</span></span>|<span data-ttu-id="2138e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2138e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2138e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2138e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2138e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2138e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2138e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2138e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2138e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2138e-115">Not supported.</span></span>|
|<span data-ttu-id="2138e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2138e-116">Application</span></span>|<span data-ttu-id="2138e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2138e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2138e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2138e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
```

## <a name="request-headers"></a><span data-ttu-id="2138e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2138e-119">Request headers</span></span>
|<span data-ttu-id="2138e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2138e-120">Header</span></span>|<span data-ttu-id="2138e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2138e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2138e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2138e-122">Authorization</span></span>|<span data-ttu-id="2138e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2138e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2138e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2138e-124">Accept</span></span>|<span data-ttu-id="2138e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2138e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2138e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2138e-126">Request body</span></span>
<span data-ttu-id="2138e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="2138e-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="2138e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplate.</span><span class="sxs-lookup"><span data-stu-id="2138e-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="2138e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2138e-129">Property</span></span>|<span data-ttu-id="2138e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2138e-130">Type</span></span>|<span data-ttu-id="2138e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2138e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2138e-132">id</span><span class="sxs-lookup"><span data-stu-id="2138e-132">id</span></span>|<span data-ttu-id="2138e-133">String</span><span class="sxs-lookup"><span data-stu-id="2138e-133">String</span></span>|<span data-ttu-id="2138e-134">A ID do modelo</span><span class="sxs-lookup"><span data-stu-id="2138e-134">The template ID</span></span>|
|<span data-ttu-id="2138e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2138e-135">displayName</span></span>|<span data-ttu-id="2138e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2138e-136">String</span></span>|<span data-ttu-id="2138e-137">O nome de exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="2138e-137">The template's display name</span></span>|
|<span data-ttu-id="2138e-138">description</span><span class="sxs-lookup"><span data-stu-id="2138e-138">description</span></span>|<span data-ttu-id="2138e-139">String</span><span class="sxs-lookup"><span data-stu-id="2138e-139">String</span></span>|<span data-ttu-id="2138e-140">A descrição do modelo</span><span class="sxs-lookup"><span data-stu-id="2138e-140">The template's description</span></span>|



## <a name="response"></a><span data-ttu-id="2138e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2138e-141">Response</span></span>
<span data-ttu-id="2138e-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2138e-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2138e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2138e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2138e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2138e-144">Request</span></span>
<span data-ttu-id="2138e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2138e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="2138e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2138e-146">Response</span></span>
<span data-ttu-id="2138e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2138e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





