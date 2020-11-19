---
title: Atualizar managedEBookCategory
description: Atualiza as propriedades de um objeto managedEBookCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d126ab73c26543815d734abf6105c932a64f555f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244756"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="d5aed-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="d5aed-103">Update managedEBookCategory</span></span>

<span data-ttu-id="d5aed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5aed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5aed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5aed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5aed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5aed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5aed-107">Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d5aed-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5aed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5aed-108">Prerequisites</span></span>
<span data-ttu-id="d5aed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5aed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5aed-111">Permission type</span></span>|<span data-ttu-id="d5aed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5aed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5aed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5aed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5aed-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5aed-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5aed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5aed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5aed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5aed-116">Not supported.</span></span>|
|<span data-ttu-id="d5aed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5aed-117">Application</span></span>|<span data-ttu-id="d5aed-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5aed-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5aed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5aed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d5aed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5aed-120">Request headers</span></span>
|<span data-ttu-id="d5aed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5aed-121">Header</span></span>|<span data-ttu-id="d5aed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5aed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5aed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5aed-123">Authorization</span></span>|<span data-ttu-id="d5aed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5aed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5aed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5aed-125">Accept</span></span>|<span data-ttu-id="d5aed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5aed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5aed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5aed-127">Request body</span></span>
<span data-ttu-id="d5aed-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d5aed-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="d5aed-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="d5aed-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="d5aed-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5aed-130">Property</span></span>|<span data-ttu-id="d5aed-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5aed-131">Type</span></span>|<span data-ttu-id="d5aed-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5aed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5aed-133">id</span><span class="sxs-lookup"><span data-stu-id="d5aed-133">id</span></span>|<span data-ttu-id="d5aed-134">String</span><span class="sxs-lookup"><span data-stu-id="d5aed-134">String</span></span>|<span data-ttu-id="d5aed-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5aed-135">The key of the entity.</span></span>|
|<span data-ttu-id="d5aed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d5aed-136">displayName</span></span>|<span data-ttu-id="d5aed-137">String</span><span class="sxs-lookup"><span data-stu-id="d5aed-137">String</span></span>|<span data-ttu-id="d5aed-138">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="d5aed-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="d5aed-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5aed-139">lastModifiedDateTime</span></span>|<span data-ttu-id="d5aed-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5aed-140">DateTimeOffset</span></span>|<span data-ttu-id="d5aed-141">A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d5aed-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d5aed-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5aed-142">Response</span></span>
<span data-ttu-id="d5aed-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5aed-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5aed-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5aed-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5aed-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5aed-145">Request</span></span>
<span data-ttu-id="d5aed-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5aed-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d5aed-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5aed-147">Response</span></span>
<span data-ttu-id="d5aed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5aed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




