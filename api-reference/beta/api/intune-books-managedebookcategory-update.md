---
title: Atualizar managedEBookCategory
description: Atualiza as propriedades de um objeto managedEBookCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 722a314f8713d9de740267eca70489b776c1cf56
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959051"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="dfea7-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="dfea7-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="dfea7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dfea7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfea7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dfea7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfea7-106">Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="dfea7-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfea7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dfea7-107">Prerequisites</span></span>
<span data-ttu-id="dfea7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfea7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfea7-110">Permission type</span></span>|<span data-ttu-id="dfea7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dfea7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfea7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfea7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfea7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfea7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dfea7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfea7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfea7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfea7-115">Not supported.</span></span>|
|<span data-ttu-id="dfea7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfea7-116">Application</span></span>|<span data-ttu-id="dfea7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfea7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfea7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfea7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="dfea7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfea7-119">Request headers</span></span>
|<span data-ttu-id="dfea7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfea7-120">Header</span></span>|<span data-ttu-id="dfea7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dfea7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfea7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfea7-122">Authorization</span></span>|<span data-ttu-id="dfea7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfea7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfea7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dfea7-124">Accept</span></span>|<span data-ttu-id="dfea7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfea7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfea7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfea7-126">Request body</span></span>
<span data-ttu-id="dfea7-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="dfea7-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="dfea7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="dfea7-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="dfea7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfea7-129">Property</span></span>|<span data-ttu-id="dfea7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfea7-130">Type</span></span>|<span data-ttu-id="dfea7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfea7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfea7-132">id</span><span class="sxs-lookup"><span data-stu-id="dfea7-132">id</span></span>|<span data-ttu-id="dfea7-133">String</span><span class="sxs-lookup"><span data-stu-id="dfea7-133">String</span></span>|<span data-ttu-id="dfea7-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dfea7-134">The key of the entity.</span></span>|
|<span data-ttu-id="dfea7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dfea7-135">displayName</span></span>|<span data-ttu-id="dfea7-136">String</span><span class="sxs-lookup"><span data-stu-id="dfea7-136">String</span></span>|<span data-ttu-id="dfea7-137">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="dfea7-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="dfea7-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfea7-138">lastModifiedDateTime</span></span>|<span data-ttu-id="dfea7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfea7-139">DateTimeOffset</span></span>|<span data-ttu-id="dfea7-140">A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dfea7-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="dfea7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfea7-141">Response</span></span>
<span data-ttu-id="dfea7-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfea7-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfea7-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfea7-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfea7-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfea7-144">Request</span></span>
<span data-ttu-id="dfea7-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfea7-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="dfea7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfea7-146">Response</span></span>
<span data-ttu-id="dfea7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfea7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





