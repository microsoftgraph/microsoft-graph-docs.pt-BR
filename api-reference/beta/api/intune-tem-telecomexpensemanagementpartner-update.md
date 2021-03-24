---
title: Atualizar telecomExpenseManagementPartner
description: Atualizar as propriedades de um objeto telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6b757c86fe3ddca1c7a86caa7c44888973a651f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123410"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="c9d97-103">Atualizar telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c9d97-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="c9d97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9d97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9d97-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9d97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9d97-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9d97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9d97-107">Atualizar as propriedades de um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c9d97-107">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9d97-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9d97-108">Prerequisites</span></span>
<span data-ttu-id="c9d97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9d97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d97-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9d97-111">Permission type</span></span>|<span data-ttu-id="c9d97-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9d97-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9d97-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9d97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9d97-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9d97-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c9d97-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9d97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9d97-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9d97-116">Not supported.</span></span>|
|<span data-ttu-id="c9d97-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9d97-117">Application</span></span>|<span data-ttu-id="c9d97-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9d97-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9d97-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9d97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="c9d97-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d97-120">Request headers</span></span>
|<span data-ttu-id="c9d97-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9d97-121">Header</span></span>|<span data-ttu-id="c9d97-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c9d97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9d97-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9d97-123">Authorization</span></span>|<span data-ttu-id="c9d97-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9d97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9d97-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9d97-125">Accept</span></span>|<span data-ttu-id="c9d97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9d97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9d97-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d97-127">Request body</span></span>
<span data-ttu-id="c9d97-128">No corpo da solicitação, forneça uma representação JSON do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c9d97-128">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="c9d97-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c9d97-129">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="c9d97-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9d97-130">Property</span></span>|<span data-ttu-id="c9d97-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9d97-131">Type</span></span>|<span data-ttu-id="c9d97-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9d97-133">id</span><span class="sxs-lookup"><span data-stu-id="c9d97-133">id</span></span>|<span data-ttu-id="c9d97-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9d97-134">String</span></span>|<span data-ttu-id="c9d97-135">O identificador exclusivo do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="c9d97-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="c9d97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c9d97-136">displayName</span></span>|<span data-ttu-id="c9d97-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9d97-137">String</span></span>|<span data-ttu-id="c9d97-138">Nome de exibição do parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="c9d97-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="c9d97-139">url</span><span class="sxs-lookup"><span data-stu-id="c9d97-139">url</span></span>|<span data-ttu-id="c9d97-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9d97-140">String</span></span>|<span data-ttu-id="c9d97-141">URL do painel de controle administrativo do parceiro TEM, em que um administrador pode configurar o serviço TEM.</span><span class="sxs-lookup"><span data-stu-id="c9d97-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="c9d97-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="c9d97-142">appAuthorized</span></span>|<span data-ttu-id="c9d97-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="c9d97-143">Boolean</span></span>|<span data-ttu-id="c9d97-144">Se aplicativo AAD do parceiro foi autorizado a acessar o Intune.</span><span class="sxs-lookup"><span data-stu-id="c9d97-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="c9d97-145">enabled</span><span class="sxs-lookup"><span data-stu-id="c9d97-145">enabled</span></span>|<span data-ttu-id="c9d97-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c9d97-146">Boolean</span></span>|<span data-ttu-id="c9d97-147">Se a conexão do Intune com o serviço TEM está habilitada ou desabilitada no momento.</span><span class="sxs-lookup"><span data-stu-id="c9d97-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="c9d97-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d97-148">lastConnectionDateTime</span></span>|<span data-ttu-id="c9d97-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9d97-149">DateTimeOffset</span></span>|<span data-ttu-id="c9d97-150">Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.</span><span class="sxs-lookup"><span data-stu-id="c9d97-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="c9d97-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d97-151">Response</span></span>
<span data-ttu-id="c9d97-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9d97-152">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9d97-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9d97-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9d97-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9d97-154">Request</span></span>
<span data-ttu-id="c9d97-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9d97-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="c9d97-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9d97-156">Response</span></span>
<span data-ttu-id="c9d97-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9d97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




