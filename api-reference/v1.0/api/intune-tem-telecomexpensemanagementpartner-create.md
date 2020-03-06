---
title: Criar telecomExpenseManagementPartner
description: Cria um novo objeto telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af8df09b4b3f13cf5b5de714d044e91b2572aad2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511926"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="11b4c-103">Criar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="11b4c-103">Create telecomExpenseManagementPartner</span></span>

<span data-ttu-id="11b4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11b4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11b4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b4c-106">Cria um novo objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="11b4c-106">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11b4c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11b4c-107">Prerequisites</span></span>
<span data-ttu-id="11b4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11b4c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11b4c-110">Permission type</span></span>|<span data-ttu-id="11b4c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11b4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11b4c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11b4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11b4c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b4c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="11b4c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11b4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11b4c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11b4c-115">Not supported.</span></span>|
|<span data-ttu-id="11b4c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11b4c-116">Application</span></span>|<span data-ttu-id="11b4c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11b4c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11b4c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11b4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="11b4c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11b4c-119">Request headers</span></span>
|<span data-ttu-id="11b4c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11b4c-120">Header</span></span>|<span data-ttu-id="11b4c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="11b4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11b4c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11b4c-122">Authorization</span></span>|<span data-ttu-id="11b4c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11b4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11b4c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11b4c-124">Accept</span></span>|<span data-ttu-id="11b4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11b4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11b4c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11b4c-126">Request body</span></span>
<span data-ttu-id="11b4c-127">No corpo da solicitação, forneça uma representação JSON do objeto telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="11b4c-127">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="11b4c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="11b4c-128">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="11b4c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11b4c-129">Property</span></span>|<span data-ttu-id="11b4c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="11b4c-130">Type</span></span>|<span data-ttu-id="11b4c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="11b4c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b4c-132">id</span><span class="sxs-lookup"><span data-stu-id="11b4c-132">id</span></span>|<span data-ttu-id="11b4c-133">String</span><span class="sxs-lookup"><span data-stu-id="11b4c-133">String</span></span>|<span data-ttu-id="11b4c-134">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="11b4c-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="11b4c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="11b4c-135">displayName</span></span>|<span data-ttu-id="11b4c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11b4c-136">String</span></span>|<span data-ttu-id="11b4c-137">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="11b4c-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="11b4c-138">url</span><span class="sxs-lookup"><span data-stu-id="11b4c-138">url</span></span>|<span data-ttu-id="11b4c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11b4c-139">String</span></span>|<span data-ttu-id="11b4c-140">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="11b4c-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="11b4c-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="11b4c-141">appAuthorized</span></span>|<span data-ttu-id="11b4c-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="11b4c-142">Boolean</span></span>|<span data-ttu-id="11b4c-143">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="11b4c-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="11b4c-144">enabled</span><span class="sxs-lookup"><span data-stu-id="11b4c-144">enabled</span></span>|<span data-ttu-id="11b4c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b4c-145">Boolean</span></span>|<span data-ttu-id="11b4c-146">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="11b4c-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="11b4c-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="11b4c-147">lastConnectionDateTime</span></span>|<span data-ttu-id="11b4c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b4c-148">DateTimeOffset</span></span>|<span data-ttu-id="11b4c-149">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="11b4c-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="11b4c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="11b4c-150">Response</span></span>
<span data-ttu-id="11b4c-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11b4c-151">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11b4c-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11b4c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="11b4c-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11b4c-153">Request</span></span>
<span data-ttu-id="11b4c-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11b4c-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="11b4c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="11b4c-155">Response</span></span>
<span data-ttu-id="11b4c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11b4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




