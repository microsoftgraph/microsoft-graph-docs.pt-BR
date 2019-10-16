---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 043611df9201c61ee696aaa6bbc986d1597b4509
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535223"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="736be-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="736be-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="736be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="736be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="736be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="736be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="736be-106">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="736be-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="736be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="736be-107">Prerequisites</span></span>
<span data-ttu-id="736be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="736be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="736be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="736be-110">Permission type</span></span>|<span data-ttu-id="736be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="736be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="736be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="736be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="736be-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="736be-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="736be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="736be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="736be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="736be-115">Not supported.</span></span>|
|<span data-ttu-id="736be-116">Application</span><span class="sxs-lookup"><span data-stu-id="736be-116">Application</span></span>|<span data-ttu-id="736be-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="736be-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="736be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="736be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="736be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="736be-119">Request headers</span></span>
|<span data-ttu-id="736be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="736be-120">Header</span></span>|<span data-ttu-id="736be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="736be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="736be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="736be-122">Authorization</span></span>|<span data-ttu-id="736be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="736be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="736be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="736be-124">Accept</span></span>|<span data-ttu-id="736be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="736be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="736be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="736be-126">Request body</span></span>
<span data-ttu-id="736be-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="736be-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="736be-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="736be-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="736be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="736be-129">Property</span></span>|<span data-ttu-id="736be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="736be-130">Type</span></span>|<span data-ttu-id="736be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="736be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="736be-132">id</span><span class="sxs-lookup"><span data-stu-id="736be-132">id</span></span>|<span data-ttu-id="736be-133">String</span><span class="sxs-lookup"><span data-stu-id="736be-133">String</span></span>|<span data-ttu-id="736be-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="736be-134">Key of the entity.</span></span> <span data-ttu-id="736be-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="736be-136">displayName</span></span>|<span data-ttu-id="736be-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-137">String</span></span>|<span data-ttu-id="736be-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="736be-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="736be-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-140">description</span><span class="sxs-lookup"><span data-stu-id="736be-140">description</span></span>|<span data-ttu-id="736be-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-141">String</span></span>|<span data-ttu-id="736be-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-142">The description of the app.</span></span> <span data-ttu-id="736be-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-144">publicador</span><span class="sxs-lookup"><span data-stu-id="736be-144">publisher</span></span>|<span data-ttu-id="736be-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-145">String</span></span>|<span data-ttu-id="736be-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-146">The publisher of the app.</span></span> <span data-ttu-id="736be-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="736be-148">largeIcon</span></span>|[<span data-ttu-id="736be-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="736be-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="736be-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="736be-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="736be-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="736be-152">createdDateTime</span></span>|<span data-ttu-id="736be-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="736be-153">DateTimeOffset</span></span>|<span data-ttu-id="736be-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-154">The date and time the app was created.</span></span> <span data-ttu-id="736be-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="736be-156">lastModifiedDateTime</span></span>|<span data-ttu-id="736be-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="736be-157">DateTimeOffset</span></span>|<span data-ttu-id="736be-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="736be-158">The date and time the app was last modified.</span></span> <span data-ttu-id="736be-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="736be-160">isFeatured</span></span>|<span data-ttu-id="736be-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="736be-161">Boolean</span></span>|<span data-ttu-id="736be-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="736be-163">privacyInformationUrl</span></span>|<span data-ttu-id="736be-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-164">String</span></span>|<span data-ttu-id="736be-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="736be-165">The privacy statement Url.</span></span> <span data-ttu-id="736be-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="736be-167">informationUrl</span></span>|<span data-ttu-id="736be-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-168">String</span></span>|<span data-ttu-id="736be-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="736be-169">The more information Url.</span></span> <span data-ttu-id="736be-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-171">owner</span><span class="sxs-lookup"><span data-stu-id="736be-171">owner</span></span>|<span data-ttu-id="736be-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-172">String</span></span>|<span data-ttu-id="736be-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="736be-173">The owner of the app.</span></span> <span data-ttu-id="736be-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-175">developer</span><span class="sxs-lookup"><span data-stu-id="736be-175">developer</span></span>|<span data-ttu-id="736be-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-176">String</span></span>|<span data-ttu-id="736be-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-177">The developer of the app.</span></span> <span data-ttu-id="736be-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-179">notes</span><span class="sxs-lookup"><span data-stu-id="736be-179">notes</span></span>|<span data-ttu-id="736be-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-180">String</span></span>|<span data-ttu-id="736be-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-181">Notes for the app.</span></span> <span data-ttu-id="736be-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="736be-183">uploadState</span></span>|<span data-ttu-id="736be-184">Int32</span><span class="sxs-lookup"><span data-stu-id="736be-184">Int32</span></span>|<span data-ttu-id="736be-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="736be-185">The upload state.</span></span> <span data-ttu-id="736be-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="736be-187">publishingState</span></span>|[<span data-ttu-id="736be-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="736be-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="736be-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-189">The publishing state for the app.</span></span> <span data-ttu-id="736be-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="736be-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="736be-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="736be-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="736be-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="736be-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="736be-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="736be-193">isAssigned</span></span>|<span data-ttu-id="736be-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="736be-194">Boolean</span></span>|<span data-ttu-id="736be-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="736be-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="736be-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="736be-197">roleScopeTagIds</span></span>|<span data-ttu-id="736be-198">String collection</span><span class="sxs-lookup"><span data-stu-id="736be-198">String collection</span></span>|<span data-ttu-id="736be-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="736be-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="736be-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="736be-201">dependentAppCount</span></span>|<span data-ttu-id="736be-202">Int32</span><span class="sxs-lookup"><span data-stu-id="736be-202">Int32</span></span>|<span data-ttu-id="736be-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="736be-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="736be-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="736be-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="736be-205">appAvailability</span></span>|[<span data-ttu-id="736be-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="736be-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="736be-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-207">The Application's availability.</span></span> <span data-ttu-id="736be-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="736be-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="736be-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="736be-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="736be-210">version</span><span class="sxs-lookup"><span data-stu-id="736be-210">version</span></span>|<span data-ttu-id="736be-211">String</span><span class="sxs-lookup"><span data-stu-id="736be-211">String</span></span>|<span data-ttu-id="736be-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="736be-212">The Application's version.</span></span> <span data-ttu-id="736be-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="736be-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="736be-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="736be-214">bundleId</span></span>|<span data-ttu-id="736be-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-215">String</span></span>|<span data-ttu-id="736be-216">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="736be-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="736be-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="736be-217">appStoreUrl</span></span>|<span data-ttu-id="736be-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="736be-218">String</span></span>|<span data-ttu-id="736be-219">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="736be-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="736be-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="736be-220">applicableDeviceType</span></span>|[<span data-ttu-id="736be-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="736be-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="736be-222">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="736be-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="736be-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="736be-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="736be-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="736be-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="736be-225">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="736be-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="736be-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="736be-226">Response</span></span>
<span data-ttu-id="736be-227">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="736be-227">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="736be-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="736be-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="736be-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="736be-229">Request</span></span>
<span data-ttu-id="736be-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="736be-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1238

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "dependentAppCount": 1,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="736be-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="736be-231">Response</span></span>
<span data-ttu-id="736be-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="736be-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1410

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "dependentAppCount": 1,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```






