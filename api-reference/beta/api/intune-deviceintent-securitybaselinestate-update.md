---
title: Atualizar securityBaselineState
description: Atualiza as propriedades de um objeto securityBaselineState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33f4a65937f8139aa7ebee483cad6e66f989caa0
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522843"
---
# <a name="update-securitybaselinestate"></a><span data-ttu-id="88a39-103">Atualizar securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="88a39-103">Update securityBaselineState</span></span>

> <span data-ttu-id="88a39-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88a39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88a39-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88a39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a39-106">Atualiza as propriedades de um objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="88a39-106">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88a39-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88a39-107">Prerequisites</span></span>
<span data-ttu-id="88a39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88a39-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88a39-110">Permission type</span></span>|<span data-ttu-id="88a39-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88a39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88a39-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88a39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88a39-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a39-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88a39-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88a39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88a39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88a39-115">Not supported.</span></span>|
|<span data-ttu-id="88a39-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88a39-116">Application</span></span>|<span data-ttu-id="88a39-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88a39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88a39-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88a39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="request-headers"></a><span data-ttu-id="88a39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88a39-119">Request headers</span></span>
|<span data-ttu-id="88a39-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88a39-120">Header</span></span>|<span data-ttu-id="88a39-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88a39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a39-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88a39-122">Authorization</span></span>|<span data-ttu-id="88a39-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88a39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a39-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88a39-124">Accept</span></span>|<span data-ttu-id="88a39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88a39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88a39-126">Request body</span></span>
<span data-ttu-id="88a39-127">No corpo da solicitação, forneça uma representação JSON do objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) .</span><span class="sxs-lookup"><span data-stu-id="88a39-127">In the request body, supply a JSON representation for the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

<span data-ttu-id="88a39-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span><span class="sxs-lookup"><span data-stu-id="88a39-128">The following table shows the properties that are required when you create the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>

|<span data-ttu-id="88a39-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88a39-129">Property</span></span>|<span data-ttu-id="88a39-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="88a39-130">Type</span></span>|<span data-ttu-id="88a39-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="88a39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a39-132">id</span><span class="sxs-lookup"><span data-stu-id="88a39-132">id</span></span>|<span data-ttu-id="88a39-133">String</span><span class="sxs-lookup"><span data-stu-id="88a39-133">String</span></span>|<span data-ttu-id="88a39-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="88a39-134">Key of the entity.</span></span>|
|<span data-ttu-id="88a39-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="88a39-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="88a39-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="88a39-136">String</span></span>|<span data-ttu-id="88a39-137">A ID do modelo de linha de base de segurança</span><span class="sxs-lookup"><span data-stu-id="88a39-137">The security baseline template id</span></span>|
|<span data-ttu-id="88a39-138">displayName</span><span class="sxs-lookup"><span data-stu-id="88a39-138">displayName</span></span>|<span data-ttu-id="88a39-139">String</span><span class="sxs-lookup"><span data-stu-id="88a39-139">String</span></span>|<span data-ttu-id="88a39-140">O nome de exibição da linha de base de segurança</span><span class="sxs-lookup"><span data-stu-id="88a39-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="88a39-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="88a39-141">Response</span></span>
<span data-ttu-id="88a39-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88a39-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a39-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88a39-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="88a39-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88a39-144">Request</span></span>
<span data-ttu-id="88a39-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88a39-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="88a39-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="88a39-146">Response</span></span>
<span data-ttu-id="88a39-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88a39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



