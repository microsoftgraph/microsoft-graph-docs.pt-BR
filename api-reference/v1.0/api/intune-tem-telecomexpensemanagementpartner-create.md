---
title: Criar telecomExpenseManagementPartner
description: Cria um novo objeto telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c244dd3cd9062439f20f1c0a5146111e6cfb775
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576567"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="04c13-103">Criar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="04c13-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="04c13-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04c13-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04c13-105">Cria um novo objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="04c13-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04c13-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04c13-106">Prerequisites</span></span>
<span data-ttu-id="04c13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04c13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04c13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04c13-109">Permission type</span></span>|<span data-ttu-id="04c13-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04c13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04c13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04c13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04c13-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04c13-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04c13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04c13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04c13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04c13-114">Not supported.</span></span>|
|<span data-ttu-id="04c13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04c13-115">Application</span></span>|<span data-ttu-id="04c13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04c13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04c13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04c13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="04c13-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04c13-118">Request headers</span></span>
|<span data-ttu-id="04c13-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04c13-119">Header</span></span>|<span data-ttu-id="04c13-120">Valor</span><span class="sxs-lookup"><span data-stu-id="04c13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04c13-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="04c13-121">Authorization</span></span>|<span data-ttu-id="04c13-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04c13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04c13-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04c13-123">Accept</span></span>|<span data-ttu-id="04c13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04c13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04c13-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04c13-125">Request body</span></span>
<span data-ttu-id="04c13-126">No corpo da solicitação, forneça uma representação JSON do objeto telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="04c13-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="04c13-127">A tabela a seguir mostra as propriedades obrigatórias ao criar telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="04c13-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="04c13-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04c13-128">Property</span></span>|<span data-ttu-id="04c13-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="04c13-129">Type</span></span>|<span data-ttu-id="04c13-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="04c13-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04c13-131">id</span><span class="sxs-lookup"><span data-stu-id="04c13-131">id</span></span>|<span data-ttu-id="04c13-132">String</span><span class="sxs-lookup"><span data-stu-id="04c13-132">String</span></span>|<span data-ttu-id="04c13-133">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="04c13-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="04c13-134">displayName</span><span class="sxs-lookup"><span data-stu-id="04c13-134">displayName</span></span>|<span data-ttu-id="04c13-135">String</span><span class="sxs-lookup"><span data-stu-id="04c13-135">String</span></span>|<span data-ttu-id="04c13-136">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="04c13-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="04c13-137">url</span><span class="sxs-lookup"><span data-stu-id="04c13-137">url</span></span>|<span data-ttu-id="04c13-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04c13-138">String</span></span>|<span data-ttu-id="04c13-139">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="04c13-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="04c13-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="04c13-140">appAuthorized</span></span>|<span data-ttu-id="04c13-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="04c13-141">Boolean</span></span>|<span data-ttu-id="04c13-142">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="04c13-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="04c13-143">enabled</span><span class="sxs-lookup"><span data-stu-id="04c13-143">enabled</span></span>|<span data-ttu-id="04c13-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="04c13-144">Boolean</span></span>|<span data-ttu-id="04c13-145">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="04c13-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="04c13-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="04c13-146">lastConnectionDateTime</span></span>|<span data-ttu-id="04c13-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04c13-147">DateTimeOffset</span></span>|<span data-ttu-id="04c13-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="04c13-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="04c13-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="04c13-149">Response</span></span>
<span data-ttu-id="04c13-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04c13-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04c13-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04c13-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="04c13-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04c13-152">Request</span></span>
<span data-ttu-id="04c13-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04c13-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04c13-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="04c13-154">Response</span></span>
<span data-ttu-id="04c13-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04c13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



