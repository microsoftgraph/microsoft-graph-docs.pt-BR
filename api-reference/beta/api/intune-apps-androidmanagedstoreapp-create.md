---
title: Criar androidManagedStoreApp
description: Criar um novo objeto androidManagedStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b69c5f734e5609b17dc76057d85278ac60fbfac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970300"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="d37e4-103">Criar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="d37e4-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="d37e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d37e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d37e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d37e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d37e4-106">Criar um novo objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d37e4-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d37e4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d37e4-107">Prerequisites</span></span>
<span data-ttu-id="d37e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d37e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d37e4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d37e4-110">Permission type</span></span>|<span data-ttu-id="d37e4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d37e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d37e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d37e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d37e4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37e4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d37e4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d37e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d37e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d37e4-115">Not supported.</span></span>|
|<span data-ttu-id="d37e4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d37e4-116">Application</span></span>|<span data-ttu-id="d37e4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d37e4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d37e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d37e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d37e4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d37e4-119">Request headers</span></span>
|<span data-ttu-id="d37e4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d37e4-120">Header</span></span>|<span data-ttu-id="d37e4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d37e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d37e4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d37e4-122">Authorization</span></span>|<span data-ttu-id="d37e4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d37e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d37e4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d37e4-124">Accept</span></span>|<span data-ttu-id="d37e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d37e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d37e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d37e4-126">Request body</span></span>
<span data-ttu-id="d37e4-127">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="d37e4-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="d37e4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="d37e4-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="d37e4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d37e4-129">Property</span></span>|<span data-ttu-id="d37e4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d37e4-130">Type</span></span>|<span data-ttu-id="d37e4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d37e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37e4-132">id</span><span class="sxs-lookup"><span data-stu-id="d37e4-132">id</span></span>|<span data-ttu-id="d37e4-133">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-133">String</span></span>|<span data-ttu-id="d37e4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d37e4-134">Key of the entity.</span></span> <span data-ttu-id="d37e4-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d37e4-136">displayName</span></span>|<span data-ttu-id="d37e4-137">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-137">String</span></span>|<span data-ttu-id="d37e4-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d37e4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d37e4-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-140">descrição</span><span class="sxs-lookup"><span data-stu-id="d37e4-140">description</span></span>|<span data-ttu-id="d37e4-141">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-141">String</span></span>|<span data-ttu-id="d37e4-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-142">The description of the app.</span></span> <span data-ttu-id="d37e4-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-144">publicador</span><span class="sxs-lookup"><span data-stu-id="d37e4-144">publisher</span></span>|<span data-ttu-id="d37e4-145">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-145">String</span></span>|<span data-ttu-id="d37e4-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-146">The publisher of the app.</span></span> <span data-ttu-id="d37e4-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d37e4-148">largeIcon</span></span>|[<span data-ttu-id="d37e4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d37e4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d37e4-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d37e4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d37e4-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d37e4-152">createdDateTime</span></span>|<span data-ttu-id="d37e4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37e4-153">DateTimeOffset</span></span>|<span data-ttu-id="d37e4-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-154">The date and time the app was created.</span></span> <span data-ttu-id="d37e4-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d37e4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d37e4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37e4-157">DateTimeOffset</span></span>|<span data-ttu-id="d37e4-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d37e4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d37e4-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d37e4-160">isFeatured</span></span>|<span data-ttu-id="d37e4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37e4-161">Boolean</span></span>|<span data-ttu-id="d37e4-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d37e4-163">privacyInformationUrl</span></span>|<span data-ttu-id="d37e4-164">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-164">String</span></span>|<span data-ttu-id="d37e4-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d37e4-165">The privacy statement Url.</span></span> <span data-ttu-id="d37e4-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d37e4-167">informationUrl</span></span>|<span data-ttu-id="d37e4-168">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-168">String</span></span>|<span data-ttu-id="d37e4-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d37e4-169">The more information Url.</span></span> <span data-ttu-id="d37e4-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-171">owner</span><span class="sxs-lookup"><span data-stu-id="d37e4-171">owner</span></span>|<span data-ttu-id="d37e4-172">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-172">String</span></span>|<span data-ttu-id="d37e4-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-173">The owner of the app.</span></span> <span data-ttu-id="d37e4-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-175">developer</span><span class="sxs-lookup"><span data-stu-id="d37e4-175">developer</span></span>|<span data-ttu-id="d37e4-176">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-176">String</span></span>|<span data-ttu-id="d37e4-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-177">The developer of the app.</span></span> <span data-ttu-id="d37e4-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-179">notes</span><span class="sxs-lookup"><span data-stu-id="d37e4-179">notes</span></span>|<span data-ttu-id="d37e4-180">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-180">String</span></span>|<span data-ttu-id="d37e4-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-181">Notes for the app.</span></span> <span data-ttu-id="d37e4-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d37e4-183">uploadState</span></span>|<span data-ttu-id="d37e4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d37e4-184">Int32</span></span>|<span data-ttu-id="d37e4-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d37e4-185">The upload state.</span></span> <span data-ttu-id="d37e4-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d37e4-187">publishingState</span></span>|[<span data-ttu-id="d37e4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d37e4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d37e4-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-189">The publishing state for the app.</span></span> <span data-ttu-id="d37e4-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d37e4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d37e4-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d37e4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d37e4-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d37e4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d37e4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d37e4-193">isAssigned</span></span>|<span data-ttu-id="d37e4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37e4-194">Boolean</span></span>|<span data-ttu-id="d37e4-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d37e4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d37e4-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d37e4-197">roleScopeTagIds</span></span>|<span data-ttu-id="d37e4-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d37e4-198">String collection</span></span>|<span data-ttu-id="d37e4-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d37e4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d37e4-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d37e4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37e4-201">packageId</span><span class="sxs-lookup"><span data-stu-id="d37e4-201">packageId</span></span>|<span data-ttu-id="d37e4-202">String</span><span class="sxs-lookup"><span data-stu-id="d37e4-202">String</span></span>|<span data-ttu-id="d37e4-203">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="d37e4-203">The package identifier.</span></span>|
|<span data-ttu-id="d37e4-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d37e4-204">appIdentifier</span></span>|<span data-ttu-id="d37e4-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d37e4-205">String</span></span>|<span data-ttu-id="d37e4-206">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="d37e4-206">The Identity Name.</span></span>|
|<span data-ttu-id="d37e4-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d37e4-207">usedLicenseCount</span></span>|<span data-ttu-id="d37e4-208">Int32</span><span class="sxs-lookup"><span data-stu-id="d37e4-208">Int32</span></span>|<span data-ttu-id="d37e4-209">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="d37e4-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="d37e4-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d37e4-210">totalLicenseCount</span></span>|<span data-ttu-id="d37e4-211">Int32</span><span class="sxs-lookup"><span data-stu-id="d37e4-211">Int32</span></span>|<span data-ttu-id="d37e4-212">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="d37e4-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="d37e4-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d37e4-213">appStoreUrl</span></span>|<span data-ttu-id="d37e4-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d37e4-214">String</span></span>|<span data-ttu-id="d37e4-215">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="d37e4-215">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="d37e4-216">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="d37e4-216">supportsOemConfig</span></span>|<span data-ttu-id="d37e4-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37e4-217">Boolean</span></span>|<span data-ttu-id="d37e4-218">Se este aplicativo dá suporte à política OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="d37e4-218">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d37e4-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="d37e4-219">Response</span></span>
<span data-ttu-id="d37e4-220">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d37e4-220">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d37e4-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d37e4-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="d37e4-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d37e4-222">Request</span></span>
<span data-ttu-id="d37e4-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d37e4-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 911

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="d37e4-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="d37e4-224">Response</span></span>
<span data-ttu-id="d37e4-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d37e4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1083

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```




