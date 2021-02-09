---
title: Atualizar windowsQualityUpdateCatalogItem
description: Atualizar as propriedades de um objeto windowsQualityUpdateCatalogItem .
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 732df024970a1e096e99e902a9b9a737a92ea3fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160121"
---
# <a name="update-windowsqualityupdatecatalogitem"></a><span data-ttu-id="d52e2-103">Atualizar windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="d52e2-103">Update windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="d52e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d52e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d52e2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d52e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d52e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d52e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d52e2-107">Atualizar as propriedades de um [objeto windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d52e2-107">Update the properties of a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d52e2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d52e2-108">Prerequisites</span></span>
<span data-ttu-id="d52e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d52e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d52e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d52e2-111">Permission type</span></span>|<span data-ttu-id="d52e2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d52e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d52e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d52e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d52e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d52e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d52e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d52e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d52e2-116">Not supported.</span></span>|
|<span data-ttu-id="d52e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d52e2-117">Application</span></span>|<span data-ttu-id="d52e2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52e2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d52e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d52e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d52e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d52e2-120">Request headers</span></span>
|<span data-ttu-id="d52e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d52e2-121">Header</span></span>|<span data-ttu-id="d52e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d52e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d52e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d52e2-123">Authorization</span></span>|<span data-ttu-id="d52e2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d52e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d52e2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d52e2-125">Accept</span></span>|<span data-ttu-id="d52e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d52e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d52e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d52e2-127">Request body</span></span>
<span data-ttu-id="d52e2-128">No corpo da solicitação, fornece uma representação JSON do [objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="d52e2-128">In the request body, supply a JSON representation for the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="d52e2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span><span class="sxs-lookup"><span data-stu-id="d52e2-129">The following table shows the properties that are required when you create the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

|<span data-ttu-id="d52e2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d52e2-130">Property</span></span>|<span data-ttu-id="d52e2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d52e2-131">Type</span></span>|<span data-ttu-id="d52e2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d52e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d52e2-133">id</span><span class="sxs-lookup"><span data-stu-id="d52e2-133">id</span></span>|<span data-ttu-id="d52e2-134">String</span><span class="sxs-lookup"><span data-stu-id="d52e2-134">String</span></span>|<span data-ttu-id="d52e2-135">A ID do item de catálogo. Herdado [de windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="d52e2-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="d52e2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d52e2-136">displayName</span></span>|<span data-ttu-id="d52e2-137">String</span><span class="sxs-lookup"><span data-stu-id="d52e2-137">String</span></span>|<span data-ttu-id="d52e2-138">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="d52e2-138">The display name for the catalog item.</span></span> <span data-ttu-id="d52e2-139">Herdado [de windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="d52e2-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="d52e2-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="d52e2-140">releaseDateTime</span></span>|<span data-ttu-id="d52e2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d52e2-141">DateTimeOffset</span></span>|<span data-ttu-id="d52e2-142">A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="d52e2-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="d52e2-143">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="d52e2-143">kbArticleId</span></span>|<span data-ttu-id="d52e2-144">String</span><span class="sxs-lookup"><span data-stu-id="d52e2-144">String</span></span>|<span data-ttu-id="d52e2-145">ID do artigo da base de dados de conhecimento</span><span class="sxs-lookup"><span data-stu-id="d52e2-145">Knowledge base article id</span></span>|
|<span data-ttu-id="d52e2-146">classificação</span><span class="sxs-lookup"><span data-stu-id="d52e2-146">classification</span></span>|[<span data-ttu-id="d52e2-147">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="d52e2-147">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="d52e2-148">Classificação da atualização de qualidade.</span><span class="sxs-lookup"><span data-stu-id="d52e2-148">Classification of the quality update.</span></span> <span data-ttu-id="d52e2-149">Os valores possíveis são: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="d52e2-149">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="d52e2-150">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="d52e2-150">isExpeditable</span></span>|<span data-ttu-id="d52e2-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d52e2-151">Boolean</span></span>|<span data-ttu-id="d52e2-152">Sinalizador indicando se a atualização se qualifica para acelerar</span><span class="sxs-lookup"><span data-stu-id="d52e2-152">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="d52e2-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d52e2-153">Response</span></span>
<span data-ttu-id="d52e2-154">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d52e2-154">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d52e2-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d52e2-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d52e2-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d52e2-156">Request</span></span>
<span data-ttu-id="d52e2-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d52e2-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
Content-type: application/json
Content-length: 272

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a><span data-ttu-id="d52e2-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d52e2-158">Response</span></span>
<span data-ttu-id="d52e2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d52e2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```




