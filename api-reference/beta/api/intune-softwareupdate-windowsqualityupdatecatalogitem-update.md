---
title: Atualizar windowsQualityUpdateCatalogItem
description: Atualize as propriedades de um objeto windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1263a65399dea4bbae5d326ca01dd0bf17c3facd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156258"
---
# <a name="update-windowsqualityupdatecatalogitem"></a><span data-ttu-id="fea6f-103">Atualizar windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="fea6f-103">Update windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="fea6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fea6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fea6f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fea6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fea6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fea6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea6f-107">Atualize as propriedades de [um objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea6f-107">Update the properties of a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fea6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fea6f-108">Prerequisites</span></span>
<span data-ttu-id="fea6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fea6f-111">Permission type</span></span>|<span data-ttu-id="fea6f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fea6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea6f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fea6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fea6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fea6f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fea6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea6f-116">Not supported.</span></span>|
|<span data-ttu-id="fea6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea6f-117">Application</span></span>|<span data-ttu-id="fea6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fea6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fea6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="fea6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6f-120">Request headers</span></span>
|<span data-ttu-id="fea6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fea6f-121">Header</span></span>|<span data-ttu-id="fea6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fea6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fea6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fea6f-123">Authorization</span></span>|<span data-ttu-id="fea6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fea6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fea6f-125">Accept</span></span>|<span data-ttu-id="fea6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fea6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6f-127">Request body</span></span>
<span data-ttu-id="fea6f-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea6f-128">In the request body, supply a JSON representation for the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="fea6f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span><span class="sxs-lookup"><span data-stu-id="fea6f-129">The following table shows the properties that are required when you create the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

|<span data-ttu-id="fea6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fea6f-130">Property</span></span>|<span data-ttu-id="fea6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fea6f-131">Type</span></span>|<span data-ttu-id="fea6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea6f-133">id</span><span class="sxs-lookup"><span data-stu-id="fea6f-133">id</span></span>|<span data-ttu-id="fea6f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fea6f-134">String</span></span>|<span data-ttu-id="fea6f-135">A ID do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea6f-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="fea6f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fea6f-136">displayName</span></span>|<span data-ttu-id="fea6f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fea6f-137">String</span></span>|<span data-ttu-id="fea6f-138">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="fea6f-138">The display name for the catalog item.</span></span> <span data-ttu-id="fea6f-139">Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea6f-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="fea6f-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="fea6f-140">releaseDateTime</span></span>|<span data-ttu-id="fea6f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea6f-141">DateTimeOffset</span></span>|<span data-ttu-id="fea6f-142">A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="fea6f-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="fea6f-143">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="fea6f-143">kbArticleId</span></span>|<span data-ttu-id="fea6f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fea6f-144">String</span></span>|<span data-ttu-id="fea6f-145">ID do artigo da base de dados de conhecimento</span><span class="sxs-lookup"><span data-stu-id="fea6f-145">Knowledge base article id</span></span>|
|<span data-ttu-id="fea6f-146">classificação</span><span class="sxs-lookup"><span data-stu-id="fea6f-146">classification</span></span>|[<span data-ttu-id="fea6f-147">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="fea6f-147">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="fea6f-148">Classificação da atualização de qualidade.</span><span class="sxs-lookup"><span data-stu-id="fea6f-148">Classification of the quality update.</span></span> <span data-ttu-id="fea6f-149">Os valores possíveis são: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="fea6f-149">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="fea6f-150">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="fea6f-150">isExpeditable</span></span>|<span data-ttu-id="fea6f-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="fea6f-151">Boolean</span></span>|<span data-ttu-id="fea6f-152">Sinalizador indicando se a atualização se qualifica para acelerar</span><span class="sxs-lookup"><span data-stu-id="fea6f-152">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="fea6f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea6f-153">Response</span></span>
<span data-ttu-id="fea6f-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fea6f-154">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fea6f-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fea6f-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="fea6f-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6f-156">Request</span></span>
<span data-ttu-id="fea6f-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fea6f-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fea6f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea6f-158">Response</span></span>
<span data-ttu-id="fea6f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fea6f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




