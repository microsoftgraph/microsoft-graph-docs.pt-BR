---
title: Atualizar managedEBookCategory
description: Atualiza as propriedades de um objeto managedEBookCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c841efbdf05f36d51c8cab26cbca84212e4241eb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776028"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="143bc-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="143bc-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="143bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="143bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="143bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="143bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="143bc-106">Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="143bc-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="143bc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="143bc-107">Prerequisites</span></span>
<span data-ttu-id="143bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="143bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="143bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="143bc-110">Permission type</span></span>|<span data-ttu-id="143bc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="143bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="143bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="143bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="143bc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="143bc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="143bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="143bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="143bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="143bc-115">Not supported.</span></span>|
|<span data-ttu-id="143bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="143bc-116">Application</span></span>|<span data-ttu-id="143bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="143bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="143bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="143bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="143bc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="143bc-119">Request headers</span></span>
|<span data-ttu-id="143bc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="143bc-120">Header</span></span>|<span data-ttu-id="143bc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="143bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="143bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="143bc-122">Authorization</span></span>|<span data-ttu-id="143bc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="143bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="143bc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="143bc-124">Accept</span></span>|<span data-ttu-id="143bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="143bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="143bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="143bc-126">Request body</span></span>
<span data-ttu-id="143bc-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="143bc-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="143bc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="143bc-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="143bc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="143bc-129">Property</span></span>|<span data-ttu-id="143bc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="143bc-130">Type</span></span>|<span data-ttu-id="143bc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="143bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="143bc-132">id</span><span class="sxs-lookup"><span data-stu-id="143bc-132">id</span></span>|<span data-ttu-id="143bc-133">String</span><span class="sxs-lookup"><span data-stu-id="143bc-133">String</span></span>|<span data-ttu-id="143bc-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="143bc-134">The key of the entity.</span></span>|
|<span data-ttu-id="143bc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="143bc-135">displayName</span></span>|<span data-ttu-id="143bc-136">String</span><span class="sxs-lookup"><span data-stu-id="143bc-136">String</span></span>|<span data-ttu-id="143bc-137">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="143bc-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="143bc-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="143bc-138">lastModifiedDateTime</span></span>|<span data-ttu-id="143bc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="143bc-139">DateTimeOffset</span></span>|<span data-ttu-id="143bc-140">A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="143bc-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="143bc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="143bc-141">Response</span></span>
<span data-ttu-id="143bc-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="143bc-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="143bc-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="143bc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="143bc-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="143bc-144">Request</span></span>
<span data-ttu-id="143bc-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="143bc-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="143bc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="143bc-146">Response</span></span>
<span data-ttu-id="143bc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="143bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





