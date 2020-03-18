---
title: Atualizar managedEBookCategory
description: Atualiza as propriedades de um objeto managedEBookCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: adc3fc59b91575723b445fe9e3667dea4fd973c7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760351"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="43847-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="43847-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="43847-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43847-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43847-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43847-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43847-106">Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="43847-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43847-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43847-107">Prerequisites</span></span>
<span data-ttu-id="43847-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43847-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43847-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43847-110">Permission type</span></span>|<span data-ttu-id="43847-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43847-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43847-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43847-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43847-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43847-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43847-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43847-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43847-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43847-115">Not supported.</span></span>|
|<span data-ttu-id="43847-116">Application</span><span class="sxs-lookup"><span data-stu-id="43847-116">Application</span></span>|<span data-ttu-id="43847-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43847-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43847-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43847-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="43847-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43847-119">Request headers</span></span>
|<span data-ttu-id="43847-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43847-120">Header</span></span>|<span data-ttu-id="43847-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43847-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43847-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43847-122">Authorization</span></span>|<span data-ttu-id="43847-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43847-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43847-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43847-124">Accept</span></span>|<span data-ttu-id="43847-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43847-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43847-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43847-126">Request body</span></span>
<span data-ttu-id="43847-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="43847-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="43847-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="43847-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="43847-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43847-129">Property</span></span>|<span data-ttu-id="43847-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="43847-130">Type</span></span>|<span data-ttu-id="43847-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="43847-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43847-132">id</span><span class="sxs-lookup"><span data-stu-id="43847-132">id</span></span>|<span data-ttu-id="43847-133">String</span><span class="sxs-lookup"><span data-stu-id="43847-133">String</span></span>|<span data-ttu-id="43847-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="43847-134">The key of the entity.</span></span>|
|<span data-ttu-id="43847-135">displayName</span><span class="sxs-lookup"><span data-stu-id="43847-135">displayName</span></span>|<span data-ttu-id="43847-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43847-136">String</span></span>|<span data-ttu-id="43847-137">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="43847-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="43847-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43847-138">lastModifiedDateTime</span></span>|<span data-ttu-id="43847-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43847-139">DateTimeOffset</span></span>|<span data-ttu-id="43847-140">A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="43847-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="43847-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="43847-141">Response</span></span>
<span data-ttu-id="43847-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43847-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43847-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43847-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="43847-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43847-144">Request</span></span>
<span data-ttu-id="43847-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43847-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="43847-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="43847-146">Response</span></span>
<span data-ttu-id="43847-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43847-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




