# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="2dc92-101">tipo enumerado managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="2dc92-101">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="2dc92-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2dc92-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dc92-103">Representa o nível ao qual a área de transferência do dispositivo pode ser compartilhada entre aplicativos</span><span class="sxs-lookup"><span data-stu-id="2dc92-103">The level to which the clipboard may be shared between apps on the managed device.</span></span>
## <a name="members"></a><span data-ttu-id="2dc92-104">Membros</span><span class="sxs-lookup"><span data-stu-id="2dc92-104">Members</span></span>
|<span data-ttu-id="2dc92-105">Membro</span><span class="sxs-lookup"><span data-stu-id="2dc92-105">Member</span></span>|<span data-ttu-id="2dc92-106">Valor</span><span class="sxs-lookup"><span data-stu-id="2dc92-106">Value</span></span>|<span data-ttu-id="2dc92-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dc92-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dc92-108">allApps</span><span class="sxs-lookup"><span data-stu-id="2dc92-108">allApps</span></span>|<span data-ttu-id="2dc92-109">0</span><span class="sxs-lookup"><span data-stu-id="2dc92-109">0%</span></span>|<span data-ttu-id="2dc92-110">O compartilhamento é permitido entre todos os aplicativos, gerenciados ou não</span><span class="sxs-lookup"><span data-stu-id="2dc92-110">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="2dc92-111">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="2dc92-111">managedAppsWithPasteIn</span></span>|<span data-ttu-id="2dc92-112">1</span><span class="sxs-lookup"><span data-stu-id="2dc92-112">-1</span></span>|<span data-ttu-id="2dc92-113">O compartilhamento é permitido entre todos os aplicativos gerenciados com a função colar habilitada</span><span class="sxs-lookup"><span data-stu-id="2dc92-113">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="2dc92-114">managedApps</span><span class="sxs-lookup"><span data-stu-id="2dc92-114">managedApps</span></span>|<span data-ttu-id="2dc92-115">2</span><span class="sxs-lookup"><span data-stu-id="2dc92-115">-2</span></span>|<span data-ttu-id="2dc92-116">O compartilhamento é permitido entre todos os aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="2dc92-116">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="2dc92-117">blocked</span><span class="sxs-lookup"><span data-stu-id="2dc92-117">Blocked</span></span>|<span data-ttu-id="2dc92-118">3</span><span class="sxs-lookup"><span data-stu-id="2dc92-118">-3</span></span>|<span data-ttu-id="2dc92-119">Compartilhamento entre aplicativos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="2dc92-119">Sharing between apps is disabled</span></span>|








