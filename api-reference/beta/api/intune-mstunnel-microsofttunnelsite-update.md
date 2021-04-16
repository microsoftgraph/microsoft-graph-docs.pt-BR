---
title: Atualizar microsoftTunnelSite
description: Atualize as propriedades de um objeto microsoftTunnelSite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74a0396c4627a8c7f4e496df78964de0ff2965cd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863826"
---
# <a name="update-microsofttunnelsite"></a><span data-ttu-id="76aa7-103">Atualizar microsoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="76aa7-103">Update microsoftTunnelSite</span></span>

<span data-ttu-id="76aa7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76aa7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76aa7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76aa7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76aa7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76aa7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76aa7-107">Atualize as propriedades de um [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)</span><span class="sxs-lookup"><span data-stu-id="76aa7-107">Update the properties of a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76aa7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76aa7-108">Prerequisites</span></span>
<span data-ttu-id="76aa7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76aa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76aa7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76aa7-111">Permission type</span></span>|<span data-ttu-id="76aa7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76aa7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76aa7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76aa7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76aa7-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76aa7-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="76aa7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76aa7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76aa7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76aa7-116">Not supported.</span></span>|
|<span data-ttu-id="76aa7-117">Application</span><span class="sxs-lookup"><span data-stu-id="76aa7-117">Application</span></span>|<span data-ttu-id="76aa7-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76aa7-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76aa7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76aa7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

## <a name="request-headers"></a><span data-ttu-id="76aa7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76aa7-120">Request headers</span></span>
|<span data-ttu-id="76aa7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76aa7-121">Header</span></span>|<span data-ttu-id="76aa7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76aa7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76aa7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76aa7-123">Authorization</span></span>|<span data-ttu-id="76aa7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76aa7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76aa7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76aa7-125">Accept</span></span>|<span data-ttu-id="76aa7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76aa7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76aa7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76aa7-127">Request body</span></span>
<span data-ttu-id="76aa7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)</span><span class="sxs-lookup"><span data-stu-id="76aa7-128">In the request body, supply a JSON representation for the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

<span data-ttu-id="76aa7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).</span><span class="sxs-lookup"><span data-stu-id="76aa7-129">The following table shows the properties that are required when you create the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).</span></span>

|<span data-ttu-id="76aa7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76aa7-130">Property</span></span>|<span data-ttu-id="76aa7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76aa7-131">Type</span></span>|<span data-ttu-id="76aa7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76aa7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76aa7-133">id</span><span class="sxs-lookup"><span data-stu-id="76aa7-133">id</span></span>|<span data-ttu-id="76aa7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76aa7-134">String</span></span>|<span data-ttu-id="76aa7-135">Id do MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="76aa7-135">The MicrosoftTunnelSite's Id</span></span>|
|<span data-ttu-id="76aa7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="76aa7-136">displayName</span></span>|<span data-ttu-id="76aa7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76aa7-137">String</span></span>|<span data-ttu-id="76aa7-138">O nome de exibição do MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="76aa7-138">The MicrosoftTunnelSite's display name</span></span>|
|<span data-ttu-id="76aa7-139">description</span><span class="sxs-lookup"><span data-stu-id="76aa7-139">description</span></span>|<span data-ttu-id="76aa7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76aa7-140">String</span></span>|<span data-ttu-id="76aa7-141">Descrição do MicrosoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="76aa7-141">The MicrosoftTunnelSite's description</span></span>|
|<span data-ttu-id="76aa7-142">publicAddress</span><span class="sxs-lookup"><span data-stu-id="76aa7-142">publicAddress</span></span>|<span data-ttu-id="76aa7-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="76aa7-143">String</span></span>|<span data-ttu-id="76aa7-144">O nome de domínio público do MicrosoftTunnelSite ou o endereço IP</span><span class="sxs-lookup"><span data-stu-id="76aa7-144">The MicrosoftTunnelSite's public domain name or IP address</span></span>|
|<span data-ttu-id="76aa7-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76aa7-145">roleScopeTagIds</span></span>|<span data-ttu-id="76aa7-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="76aa7-146">String collection</span></span>|<span data-ttu-id="76aa7-147">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="76aa7-147">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="76aa7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="76aa7-148">Response</span></span>
<span data-ttu-id="76aa7-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76aa7-149">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76aa7-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76aa7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="76aa7-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76aa7-151">Request</span></span>
<span data-ttu-id="76aa7-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76aa7-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
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

### <a name="response"></a><span data-ttu-id="76aa7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="76aa7-153">Response</span></span>
<span data-ttu-id="76aa7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76aa7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




