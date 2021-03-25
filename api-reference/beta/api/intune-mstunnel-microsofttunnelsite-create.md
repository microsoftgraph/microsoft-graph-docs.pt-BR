---
title: Criar microsoftTunnelSite
description: Crie um novo objeto microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f8f6eb29565ead693cc94d95cb0ad59ba4e15e7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152961"
---
# <a name="create-microsofttunnelsite"></a><span data-ttu-id="cc98e-103">Criar microsoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="cc98e-103">Create microsoftTunnelSite</span></span>

<span data-ttu-id="cc98e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc98e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc98e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc98e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc98e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc98e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc98e-107">Crie um novo [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)</span><span class="sxs-lookup"><span data-stu-id="cc98e-107">Create a new [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc98e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc98e-108">Prerequisites</span></span>
<span data-ttu-id="cc98e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc98e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc98e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc98e-111">Permission type</span></span>|<span data-ttu-id="cc98e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc98e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc98e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc98e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc98e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc98e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc98e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc98e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc98e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc98e-116">Not supported.</span></span>|
|<span data-ttu-id="cc98e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc98e-117">Application</span></span>|<span data-ttu-id="cc98e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc98e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc98e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc98e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a><span data-ttu-id="cc98e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc98e-120">Request headers</span></span>
|<span data-ttu-id="cc98e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc98e-121">Header</span></span>|<span data-ttu-id="cc98e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cc98e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc98e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc98e-123">Authorization</span></span>|<span data-ttu-id="cc98e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc98e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc98e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc98e-125">Accept</span></span>|<span data-ttu-id="cc98e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc98e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc98e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc98e-127">Request body</span></span>
<span data-ttu-id="cc98e-128">No corpo da solicitação, fornece uma representação JSON para o objeto microsoftTunnelSite.</span><span class="sxs-lookup"><span data-stu-id="cc98e-128">In the request body, supply a JSON representation for the microsoftTunnelSite object.</span></span>

<span data-ttu-id="cc98e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o microsoftTunnelSite.</span><span class="sxs-lookup"><span data-stu-id="cc98e-129">The following table shows the properties that are required when you create the microsoftTunnelSite.</span></span>

|<span data-ttu-id="cc98e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc98e-130">Property</span></span>|<span data-ttu-id="cc98e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc98e-131">Type</span></span>|<span data-ttu-id="cc98e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc98e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc98e-133">id</span><span class="sxs-lookup"><span data-stu-id="cc98e-133">id</span></span>|<span data-ttu-id="cc98e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc98e-134">String</span></span>|<span data-ttu-id="cc98e-135">Id do MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="cc98e-135">The MicrosoftTunnelSite's Id</span></span>|
|<span data-ttu-id="cc98e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cc98e-136">displayName</span></span>|<span data-ttu-id="cc98e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc98e-137">String</span></span>|<span data-ttu-id="cc98e-138">O nome de exibição do MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="cc98e-138">The MicrosoftTunnelSite's display name</span></span>|
|<span data-ttu-id="cc98e-139">descrição</span><span class="sxs-lookup"><span data-stu-id="cc98e-139">description</span></span>|<span data-ttu-id="cc98e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc98e-140">String</span></span>|<span data-ttu-id="cc98e-141">Descrição do MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="cc98e-141">The MicrosoftTunnelSite's description</span></span>|
|<span data-ttu-id="cc98e-142">publicAddress</span><span class="sxs-lookup"><span data-stu-id="cc98e-142">publicAddress</span></span>|<span data-ttu-id="cc98e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc98e-143">String</span></span>|<span data-ttu-id="cc98e-144">O nome de domínio público do MicrosoftTunnelSite ou o endereço IP</span><span class="sxs-lookup"><span data-stu-id="cc98e-144">The MicrosoftTunnelSite's public domain name or IP address</span></span>|
|<span data-ttu-id="cc98e-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc98e-145">roleScopeTagIds</span></span>|<span data-ttu-id="cc98e-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc98e-146">String collection</span></span>|<span data-ttu-id="cc98e-147">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="cc98e-147">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cc98e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc98e-148">Response</span></span>
<span data-ttu-id="cc98e-149">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc98e-149">If successful, this method returns a `201 Created` response code and a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc98e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc98e-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc98e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc98e-151">Request</span></span>
<span data-ttu-id="cc98e-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc98e-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cc98e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc98e-153">Response</span></span>
<span data-ttu-id="cc98e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc98e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




