---
title: Criar windowsQualityUpdateCatalogItem
description: Crie um novo objeto windowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aec5d998ed02c946059816d164188bb566ddec7e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866878"
---
# <a name="create-windowsqualityupdatecatalogitem"></a><span data-ttu-id="6bf2e-103">Criar windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="6bf2e-103">Create windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="6bf2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bf2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bf2e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bf2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bf2e-107">Crie um novo [objeto windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-107">Create a new [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bf2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bf2e-108">Prerequisites</span></span>
<span data-ttu-id="6bf2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bf2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bf2e-111">Permission type</span></span>|<span data-ttu-id="6bf2e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bf2e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bf2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bf2e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bf2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-116">Not supported.</span></span>|
|<span data-ttu-id="6bf2e-117">Application</span><span class="sxs-lookup"><span data-stu-id="6bf2e-117">Application</span></span>|<span data-ttu-id="6bf2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bf2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bf2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="6bf2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bf2e-120">Request headers</span></span>
|<span data-ttu-id="6bf2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bf2e-121">Header</span></span>|<span data-ttu-id="6bf2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6bf2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bf2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bf2e-123">Authorization</span></span>|<span data-ttu-id="6bf2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bf2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bf2e-125">Accept</span></span>|<span data-ttu-id="6bf2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bf2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bf2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bf2e-127">Request body</span></span>
<span data-ttu-id="6bf2e-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsQualityUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-128">In the request body, supply a JSON representation for the windowsQualityUpdateCatalogItem object.</span></span>

<span data-ttu-id="6bf2e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsQualityUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-129">The following table shows the properties that are required when you create the windowsQualityUpdateCatalogItem.</span></span>

|<span data-ttu-id="6bf2e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bf2e-130">Property</span></span>|<span data-ttu-id="6bf2e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bf2e-131">Type</span></span>|<span data-ttu-id="6bf2e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bf2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf2e-133">id</span><span class="sxs-lookup"><span data-stu-id="6bf2e-133">id</span></span>|<span data-ttu-id="6bf2e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bf2e-134">String</span></span>|<span data-ttu-id="6bf2e-135">A ID do item de catálogo. Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="6bf2e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6bf2e-136">displayName</span></span>|<span data-ttu-id="6bf2e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bf2e-137">String</span></span>|<span data-ttu-id="6bf2e-138">O nome de exibição do item de catálogo.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-138">The display name for the catalog item.</span></span> <span data-ttu-id="6bf2e-139">Herdado [do windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="6bf2e-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="6bf2e-140">releaseDateTime</span></span>|<span data-ttu-id="6bf2e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bf2e-141">DateTimeOffset</span></span>|<span data-ttu-id="6bf2e-142">A data em que o item de catálogo foi lançado Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="6bf2e-143">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="6bf2e-143">endOfSupportDate</span></span>|<span data-ttu-id="6bf2e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bf2e-144">DateTimeOffset</span></span>|<span data-ttu-id="6bf2e-145">A última data com suporte para um item de catálogo Herdado de [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="6bf2e-145">The last supported date for a catalog item Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="6bf2e-146">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="6bf2e-146">kbArticleId</span></span>|<span data-ttu-id="6bf2e-147">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="6bf2e-147">String</span></span>|<span data-ttu-id="6bf2e-148">ID do artigo da base de dados de conhecimento</span><span class="sxs-lookup"><span data-stu-id="6bf2e-148">Knowledge base article id</span></span>|
|<span data-ttu-id="6bf2e-149">classificação</span><span class="sxs-lookup"><span data-stu-id="6bf2e-149">classification</span></span>|[<span data-ttu-id="6bf2e-150">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="6bf2e-150">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="6bf2e-151">Classificação da atualização de qualidade.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-151">Classification of the quality update.</span></span> <span data-ttu-id="6bf2e-152">Os valores possíveis são: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-152">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="6bf2e-153">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="6bf2e-153">isExpeditable</span></span>|<span data-ttu-id="6bf2e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bf2e-154">Boolean</span></span>|<span data-ttu-id="6bf2e-155">Sinalizador indicando se a atualização se qualifica para acelerar</span><span class="sxs-lookup"><span data-stu-id="6bf2e-155">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="6bf2e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bf2e-156">Response</span></span>
<span data-ttu-id="6bf2e-157">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-157">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bf2e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bf2e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bf2e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bf2e-159">Request</span></span>
<span data-ttu-id="6bf2e-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a><span data-ttu-id="6bf2e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bf2e-161">Response</span></span>
<span data-ttu-id="6bf2e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bf2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 381

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```




