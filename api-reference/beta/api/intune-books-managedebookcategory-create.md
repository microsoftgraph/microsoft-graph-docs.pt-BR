---
title: Criar managedEBookCategory
description: Crie um novo objeto managedEBookCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae2fd38c576d2d85f4d07137a17e3a20be78ccff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133028"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="318e1-103">Criar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="318e1-103">Create managedEBookCategory</span></span>

<span data-ttu-id="318e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="318e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="318e1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="318e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="318e1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="318e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="318e1-107">Crie um novo [objeto managedEBookCategory.](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="318e1-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="318e1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="318e1-108">Prerequisites</span></span>
<span data-ttu-id="318e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="318e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="318e1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="318e1-111">Permission type</span></span>|<span data-ttu-id="318e1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="318e1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="318e1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="318e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="318e1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318e1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="318e1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="318e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="318e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="318e1-116">Not supported.</span></span>|
|<span data-ttu-id="318e1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="318e1-117">Application</span></span>|<span data-ttu-id="318e1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318e1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="318e1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="318e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="318e1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="318e1-120">Request headers</span></span>
|<span data-ttu-id="318e1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="318e1-121">Header</span></span>|<span data-ttu-id="318e1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="318e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="318e1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="318e1-123">Authorization</span></span>|<span data-ttu-id="318e1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="318e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="318e1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="318e1-125">Accept</span></span>|<span data-ttu-id="318e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="318e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="318e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="318e1-127">Request body</span></span>
<span data-ttu-id="318e1-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="318e1-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="318e1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="318e1-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="318e1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="318e1-130">Property</span></span>|<span data-ttu-id="318e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="318e1-131">Type</span></span>|<span data-ttu-id="318e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="318e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="318e1-133">id</span><span class="sxs-lookup"><span data-stu-id="318e1-133">id</span></span>|<span data-ttu-id="318e1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="318e1-134">String</span></span>|<span data-ttu-id="318e1-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="318e1-135">The key of the entity.</span></span>|
|<span data-ttu-id="318e1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="318e1-136">displayName</span></span>|<span data-ttu-id="318e1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="318e1-137">String</span></span>|<span data-ttu-id="318e1-138">O nome da categoria de eBook.</span><span class="sxs-lookup"><span data-stu-id="318e1-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="318e1-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="318e1-139">lastModifiedDateTime</span></span>|<span data-ttu-id="318e1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="318e1-140">DateTimeOffset</span></span>|<span data-ttu-id="318e1-141">A data e a hora em que ManagedEBookCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="318e1-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="318e1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="318e1-142">Response</span></span>
<span data-ttu-id="318e1-143">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="318e1-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="318e1-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="318e1-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="318e1-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="318e1-145">Request</span></span>
<span data-ttu-id="318e1-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="318e1-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="318e1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="318e1-147">Response</span></span>
<span data-ttu-id="318e1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="318e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




