---
title: Criar telecomExpenseManagementPartner
description: Cria um novo objeto telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c83b26e0f9d9c2a881ca37a4a56c2cc37883120
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262325"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="b6d18-103">Criar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b6d18-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="b6d18-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6d18-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6d18-105">Cria um novo objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b6d18-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6d18-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6d18-106">Prerequisites</span></span>
<span data-ttu-id="b6d18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6d18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6d18-109">Permission type</span></span>|<span data-ttu-id="b6d18-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6d18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6d18-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6d18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6d18-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d18-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6d18-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6d18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6d18-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6d18-114">Not supported.</span></span>|
|<span data-ttu-id="b6d18-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6d18-115">Application</span></span>|<span data-ttu-id="b6d18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6d18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6d18-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="b6d18-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d18-118">Request headers</span></span>
|<span data-ttu-id="b6d18-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6d18-119">Header</span></span>|<span data-ttu-id="b6d18-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b6d18-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6d18-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6d18-121">Authorization</span></span>|<span data-ttu-id="b6d18-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6d18-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6d18-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6d18-123">Accept</span></span>|<span data-ttu-id="b6d18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b6d18-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6d18-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d18-125">Request body</span></span>
<span data-ttu-id="b6d18-126">No corpo da solicitação, forneça uma representação JSON do objeto telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="b6d18-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="b6d18-127">A tabela a seguir mostra as propriedades obrigatórias ao criar telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="b6d18-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="b6d18-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6d18-128">Property</span></span>|<span data-ttu-id="b6d18-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d18-129">Type</span></span>|<span data-ttu-id="b6d18-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d18-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6d18-131">id</span><span class="sxs-lookup"><span data-stu-id="b6d18-131">id</span></span>|<span data-ttu-id="b6d18-132">String</span><span class="sxs-lookup"><span data-stu-id="b6d18-132">String</span></span>|<span data-ttu-id="b6d18-133">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="b6d18-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="b6d18-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b6d18-134">displayName</span></span>|<span data-ttu-id="b6d18-135">String</span><span class="sxs-lookup"><span data-stu-id="b6d18-135">String</span></span>|<span data-ttu-id="b6d18-136">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="b6d18-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="b6d18-137">url</span><span class="sxs-lookup"><span data-stu-id="b6d18-137">url</span></span>|<span data-ttu-id="b6d18-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6d18-138">String</span></span>|<span data-ttu-id="b6d18-139">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="b6d18-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="b6d18-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="b6d18-140">appAuthorized</span></span>|<span data-ttu-id="b6d18-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6d18-141">Boolean</span></span>|<span data-ttu-id="b6d18-142">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="b6d18-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="b6d18-143">enabled</span><span class="sxs-lookup"><span data-stu-id="b6d18-143">enabled</span></span>|<span data-ttu-id="b6d18-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6d18-144">Boolean</span></span>|<span data-ttu-id="b6d18-145">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="b6d18-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="b6d18-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b6d18-146">lastConnectionDateTime</span></span>|<span data-ttu-id="b6d18-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6d18-147">DateTimeOffset</span></span>|<span data-ttu-id="b6d18-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="b6d18-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="b6d18-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d18-149">Response</span></span>
<span data-ttu-id="b6d18-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d18-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6d18-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6d18-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6d18-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d18-152">Request</span></span>
<span data-ttu-id="b6d18-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6d18-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6d18-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d18-154">Response</span></span>
<span data-ttu-id="b6d18-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6d18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



