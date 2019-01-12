---
title: Criar telecomExpenseManagementPartner
description: Cria um novo objeto telecomExpenseManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ca3a94da0c908bec0af44075dcb15b6fa4f007a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984798"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="90aae-103">Criar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="90aae-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="90aae-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="90aae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90aae-105">Cria um novo objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="90aae-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90aae-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90aae-106">Prerequisites</span></span>
<span data-ttu-id="90aae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90aae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90aae-109">Permission type</span></span>|<span data-ttu-id="90aae-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90aae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90aae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90aae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90aae-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90aae-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90aae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90aae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90aae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90aae-114">Not supported.</span></span>|
|<span data-ttu-id="90aae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90aae-115">Application</span></span>|<span data-ttu-id="90aae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90aae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90aae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90aae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="90aae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90aae-118">Request headers</span></span>
|<span data-ttu-id="90aae-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90aae-119">Header</span></span>|<span data-ttu-id="90aae-120">Valor</span><span class="sxs-lookup"><span data-stu-id="90aae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90aae-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="90aae-121">Authorization</span></span>|<span data-ttu-id="90aae-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90aae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90aae-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90aae-123">Accept</span></span>|<span data-ttu-id="90aae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90aae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90aae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90aae-125">Request body</span></span>
<span data-ttu-id="90aae-126">No corpo da solicitação, forneça uma representação JSON do objeto telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="90aae-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="90aae-127">A tabela a seguir mostra as propriedades obrigatórias ao criar telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="90aae-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="90aae-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90aae-128">Property</span></span>|<span data-ttu-id="90aae-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="90aae-129">Type</span></span>|<span data-ttu-id="90aae-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="90aae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90aae-131">id</span><span class="sxs-lookup"><span data-stu-id="90aae-131">id</span></span>|<span data-ttu-id="90aae-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90aae-132">String</span></span>|<span data-ttu-id="90aae-133">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="90aae-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="90aae-134">displayName</span><span class="sxs-lookup"><span data-stu-id="90aae-134">displayName</span></span>|<span data-ttu-id="90aae-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90aae-135">String</span></span>|<span data-ttu-id="90aae-136">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="90aae-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="90aae-137">url</span><span class="sxs-lookup"><span data-stu-id="90aae-137">url</span></span>|<span data-ttu-id="90aae-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90aae-138">String</span></span>|<span data-ttu-id="90aae-139">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="90aae-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="90aae-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="90aae-140">appAuthorized</span></span>|<span data-ttu-id="90aae-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="90aae-141">Boolean</span></span>|<span data-ttu-id="90aae-142">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="90aae-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="90aae-143">enabled</span><span class="sxs-lookup"><span data-stu-id="90aae-143">enabled</span></span>|<span data-ttu-id="90aae-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="90aae-144">Boolean</span></span>|<span data-ttu-id="90aae-145">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="90aae-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="90aae-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="90aae-146">lastConnectionDateTime</span></span>|<span data-ttu-id="90aae-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90aae-147">DateTimeOffset</span></span>|<span data-ttu-id="90aae-148">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="90aae-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="90aae-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="90aae-149">Response</span></span>
<span data-ttu-id="90aae-150">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90aae-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90aae-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90aae-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="90aae-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90aae-152">Request</span></span>
<span data-ttu-id="90aae-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90aae-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90aae-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="90aae-154">Response</span></span>
<span data-ttu-id="90aae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90aae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



