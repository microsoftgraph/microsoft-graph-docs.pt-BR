---
title: Atualizar managedEBookCategory
description: Atualiza as propriedades de um objeto managedEBookCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dad9d166fafb2ad945c99def4280e0948790ac4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690193"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="4a674-103">Atualizar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="4a674-103">Update managedEBookCategory</span></span>

<span data-ttu-id="4a674-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a674-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a674-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a674-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a674-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a674-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a674-107">Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="4a674-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a674-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a674-108">Prerequisites</span></span>
<span data-ttu-id="4a674-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a674-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a674-111">Permission type</span></span>|<span data-ttu-id="4a674-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a674-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a674-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a674-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a674-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a674-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a674-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a674-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a674-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a674-116">Not supported.</span></span>|
|<span data-ttu-id="4a674-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a674-117">Application</span></span>|<span data-ttu-id="4a674-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a674-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a674-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a674-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="4a674-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a674-120">Request headers</span></span>
|<span data-ttu-id="4a674-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a674-121">Header</span></span>|<span data-ttu-id="4a674-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a674-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a674-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a674-123">Authorization</span></span>|<span data-ttu-id="4a674-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a674-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a674-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a674-125">Accept</span></span>|<span data-ttu-id="4a674-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a674-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a674-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a674-127">Request body</span></span>
<span data-ttu-id="4a674-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="4a674-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="4a674-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="4a674-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="4a674-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a674-130">Property</span></span>|<span data-ttu-id="4a674-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a674-131">Type</span></span>|<span data-ttu-id="4a674-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a674-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a674-133">id</span><span class="sxs-lookup"><span data-stu-id="4a674-133">id</span></span>|<span data-ttu-id="4a674-134">String</span><span class="sxs-lookup"><span data-stu-id="4a674-134">String</span></span>|<span data-ttu-id="4a674-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a674-135">The key of the entity.</span></span>|
|<span data-ttu-id="4a674-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4a674-136">displayName</span></span>|<span data-ttu-id="4a674-137">String</span><span class="sxs-lookup"><span data-stu-id="4a674-137">String</span></span>|<span data-ttu-id="4a674-138">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="4a674-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="4a674-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a674-139">lastModifiedDateTime</span></span>|<span data-ttu-id="4a674-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a674-140">DateTimeOffset</span></span>|<span data-ttu-id="4a674-141">A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4a674-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="4a674-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a674-142">Response</span></span>
<span data-ttu-id="4a674-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a674-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a674-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a674-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a674-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a674-145">Request</span></span>
<span data-ttu-id="4a674-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a674-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4a674-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a674-147">Response</span></span>
<span data-ttu-id="4a674-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a674-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





