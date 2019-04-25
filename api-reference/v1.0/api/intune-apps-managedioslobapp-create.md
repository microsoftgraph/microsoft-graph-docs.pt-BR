---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a58dcbdabcd879d6a5164bbf830df9de6fc24c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578075"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="7aa99-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="7aa99-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="7aa99-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7aa99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aa99-105">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7aa99-105">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7aa99-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7aa99-106">Prerequisites</span></span>
<span data-ttu-id="7aa99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aa99-109">Permission type</span></span>|<span data-ttu-id="7aa99-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7aa99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aa99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aa99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7aa99-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa99-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7aa99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aa99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aa99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aa99-114">Not supported.</span></span>|
|<span data-ttu-id="7aa99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aa99-115">Application</span></span>|<span data-ttu-id="7aa99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aa99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aa99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aa99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7aa99-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa99-118">Request headers</span></span>
|<span data-ttu-id="7aa99-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7aa99-119">Header</span></span>|<span data-ttu-id="7aa99-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7aa99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aa99-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aa99-121">Authorization</span></span>|<span data-ttu-id="7aa99-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aa99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aa99-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7aa99-123">Accept</span></span>|<span data-ttu-id="7aa99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7aa99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aa99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa99-125">Request body</span></span>
<span data-ttu-id="7aa99-126">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="7aa99-126">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="7aa99-127">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="7aa99-127">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="7aa99-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aa99-128">Property</span></span>|<span data-ttu-id="7aa99-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aa99-129">Type</span></span>|<span data-ttu-id="7aa99-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aa99-131">id</span><span class="sxs-lookup"><span data-stu-id="7aa99-131">id</span></span>|<span data-ttu-id="7aa99-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aa99-132">String</span></span>|<span data-ttu-id="7aa99-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7aa99-133">Key of the entity.</span></span> <span data-ttu-id="7aa99-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7aa99-135">displayName</span></span>|<span data-ttu-id="7aa99-136">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-136">String</span></span>|<span data-ttu-id="7aa99-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7aa99-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7aa99-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-139">description</span><span class="sxs-lookup"><span data-stu-id="7aa99-139">description</span></span>|<span data-ttu-id="7aa99-140">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-140">String</span></span>|<span data-ttu-id="7aa99-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-141">The description of the app.</span></span> <span data-ttu-id="7aa99-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-143">publicador</span><span class="sxs-lookup"><span data-stu-id="7aa99-143">publisher</span></span>|<span data-ttu-id="7aa99-144">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-144">String</span></span>|<span data-ttu-id="7aa99-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-145">The publisher of the app.</span></span> <span data-ttu-id="7aa99-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7aa99-147">largeIcon</span></span>|[<span data-ttu-id="7aa99-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7aa99-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7aa99-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7aa99-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7aa99-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa99-151">createdDateTime</span></span>|<span data-ttu-id="7aa99-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa99-152">DateTimeOffset</span></span>|<span data-ttu-id="7aa99-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-153">The date and time the app was created.</span></span> <span data-ttu-id="7aa99-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa99-155">lastModifiedDateTime</span></span>|<span data-ttu-id="7aa99-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa99-156">DateTimeOffset</span></span>|<span data-ttu-id="7aa99-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7aa99-157">The date and time the app was last modified.</span></span> <span data-ttu-id="7aa99-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7aa99-159">isFeatured</span></span>|<span data-ttu-id="7aa99-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7aa99-160">Boolean</span></span>|<span data-ttu-id="7aa99-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7aa99-162">privacyInformationUrl</span></span>|<span data-ttu-id="7aa99-163">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-163">String</span></span>|<span data-ttu-id="7aa99-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7aa99-164">The privacy statement Url.</span></span> <span data-ttu-id="7aa99-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7aa99-166">informationUrl</span></span>|<span data-ttu-id="7aa99-167">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-167">String</span></span>|<span data-ttu-id="7aa99-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7aa99-168">The more information Url.</span></span> <span data-ttu-id="7aa99-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-170">owner</span><span class="sxs-lookup"><span data-stu-id="7aa99-170">owner</span></span>|<span data-ttu-id="7aa99-171">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-171">String</span></span>|<span data-ttu-id="7aa99-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-172">The owner of the app.</span></span> <span data-ttu-id="7aa99-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-174">developer</span><span class="sxs-lookup"><span data-stu-id="7aa99-174">developer</span></span>|<span data-ttu-id="7aa99-175">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-175">String</span></span>|<span data-ttu-id="7aa99-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-176">The developer of the app.</span></span> <span data-ttu-id="7aa99-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-178">notes</span><span class="sxs-lookup"><span data-stu-id="7aa99-178">notes</span></span>|<span data-ttu-id="7aa99-179">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-179">String</span></span>|<span data-ttu-id="7aa99-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-180">Notes for the app.</span></span> <span data-ttu-id="7aa99-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7aa99-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="7aa99-182">publishingState</span></span>|[<span data-ttu-id="7aa99-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7aa99-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7aa99-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-184">The publishing state for the app.</span></span> <span data-ttu-id="7aa99-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7aa99-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7aa99-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7aa99-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7aa99-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7aa99-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7aa99-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7aa99-188">appAvailability</span></span>|[<span data-ttu-id="7aa99-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="7aa99-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="7aa99-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-190">The Application's availability.</span></span> <span data-ttu-id="7aa99-191">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7aa99-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="7aa99-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="7aa99-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7aa99-193">version</span><span class="sxs-lookup"><span data-stu-id="7aa99-193">version</span></span>|<span data-ttu-id="7aa99-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aa99-194">String</span></span>|<span data-ttu-id="7aa99-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7aa99-195">The Application's version.</span></span> <span data-ttu-id="7aa99-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="7aa99-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7aa99-197">committedContentVersion</span></span>|<span data-ttu-id="7aa99-198">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-198">String</span></span>|<span data-ttu-id="7aa99-199">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="7aa99-199">The internal committed content version.</span></span> <span data-ttu-id="7aa99-200">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7aa99-201">fileName</span><span class="sxs-lookup"><span data-stu-id="7aa99-201">fileName</span></span>|<span data-ttu-id="7aa99-202">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-202">String</span></span>|<span data-ttu-id="7aa99-203">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="7aa99-203">The name of the main Lob application file.</span></span> <span data-ttu-id="7aa99-204">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7aa99-205">size</span><span class="sxs-lookup"><span data-stu-id="7aa99-205">size</span></span>|<span data-ttu-id="7aa99-206">Int64</span><span class="sxs-lookup"><span data-stu-id="7aa99-206">Int64</span></span>|<span data-ttu-id="7aa99-207">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="7aa99-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="7aa99-208">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7aa99-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7aa99-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="7aa99-209">bundleId</span></span>|<span data-ttu-id="7aa99-210">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-210">String</span></span>|<span data-ttu-id="7aa99-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7aa99-211">The Identity Name.</span></span>|
|<span data-ttu-id="7aa99-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="7aa99-212">applicableDeviceType</span></span>|[<span data-ttu-id="7aa99-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7aa99-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="7aa99-214">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="7aa99-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="7aa99-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7aa99-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7aa99-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7aa99-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="7aa99-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="7aa99-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7aa99-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa99-218">expirationDateTime</span></span>|<span data-ttu-id="7aa99-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa99-219">DateTimeOffset</span></span>|<span data-ttu-id="7aa99-220">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="7aa99-220">The expiration time.</span></span>|
|<span data-ttu-id="7aa99-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="7aa99-221">versionNumber</span></span>|<span data-ttu-id="7aa99-222">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-222">String</span></span>|<span data-ttu-id="7aa99-223">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7aa99-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7aa99-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="7aa99-224">buildNumber</span></span>|<span data-ttu-id="7aa99-225">String</span><span class="sxs-lookup"><span data-stu-id="7aa99-225">String</span></span>|<span data-ttu-id="7aa99-226">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7aa99-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="7aa99-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa99-227">Response</span></span>
<span data-ttu-id="7aa99-228">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aa99-228">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa99-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7aa99-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="7aa99-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aa99-230">Request</span></span>
<span data-ttu-id="7aa99-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aa99-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="7aa99-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aa99-232">Response</span></span>
<span data-ttu-id="7aa99-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aa99-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



