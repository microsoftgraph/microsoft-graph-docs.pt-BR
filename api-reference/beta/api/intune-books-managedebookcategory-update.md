---
title: Atualizar managedEBookCategory
description: Atualiza as propriedades de um objeto managedEBookCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbc5436c7f4140d1c2cd517b42468b67109c6fd5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43414092"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="f7312-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="f7312-103">Update managedEBookCategory</span></span>

<span data-ttu-id="f7312-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7312-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7312-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7312-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7312-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7312-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7312-107">Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f7312-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7312-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7312-108">Prerequisites</span></span>
<span data-ttu-id="f7312-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7312-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7312-111">Permission type</span></span>|<span data-ttu-id="f7312-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7312-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7312-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7312-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7312-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7312-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7312-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7312-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7312-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7312-116">Not supported.</span></span>|
|<span data-ttu-id="f7312-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7312-117">Application</span></span>|<span data-ttu-id="f7312-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7312-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7312-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7312-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f7312-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7312-120">Request headers</span></span>
|<span data-ttu-id="f7312-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7312-121">Header</span></span>|<span data-ttu-id="f7312-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7312-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7312-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7312-123">Authorization</span></span>|<span data-ttu-id="f7312-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7312-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7312-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7312-125">Accept</span></span>|<span data-ttu-id="f7312-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7312-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7312-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7312-127">Request body</span></span>
<span data-ttu-id="f7312-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f7312-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="f7312-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f7312-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="f7312-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7312-130">Property</span></span>|<span data-ttu-id="f7312-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7312-131">Type</span></span>|<span data-ttu-id="f7312-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7312-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7312-133">id</span><span class="sxs-lookup"><span data-stu-id="f7312-133">id</span></span>|<span data-ttu-id="f7312-134">String</span><span class="sxs-lookup"><span data-stu-id="f7312-134">String</span></span>|<span data-ttu-id="f7312-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7312-135">The key of the entity.</span></span>|
|<span data-ttu-id="f7312-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f7312-136">displayName</span></span>|<span data-ttu-id="f7312-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7312-137">String</span></span>|<span data-ttu-id="f7312-138">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="f7312-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="f7312-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7312-139">lastModifiedDateTime</span></span>|<span data-ttu-id="f7312-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7312-140">DateTimeOffset</span></span>|<span data-ttu-id="f7312-141">A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f7312-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="f7312-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7312-142">Response</span></span>
<span data-ttu-id="f7312-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7312-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7312-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7312-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7312-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7312-145">Request</span></span>
<span data-ttu-id="f7312-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7312-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="f7312-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7312-147">Response</span></span>
<span data-ttu-id="f7312-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7312-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



