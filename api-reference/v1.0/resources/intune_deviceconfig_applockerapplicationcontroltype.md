# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0165d-101">tipo enumumerado appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="0165d-101">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0165d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0165d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0165d-103">Valores possíveis de tipos de controle do aplicativo AppLocker</span><span class="sxs-lookup"><span data-stu-id="0165d-103">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="0165d-104">Membros</span><span class="sxs-lookup"><span data-stu-id="0165d-104">Members</span></span>
|<span data-ttu-id="0165d-105">Membro</span><span class="sxs-lookup"><span data-stu-id="0165d-105">Member</span></span>|<span data-ttu-id="0165d-106">Valor</span><span class="sxs-lookup"><span data-stu-id="0165d-106">Value</span></span>|<span data-ttu-id="0165d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0165d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0165d-108">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="0165d-108">notConfigured</span></span>|<span data-ttu-id="0165d-109">0</span><span class="sxs-lookup"><span data-stu-id="0165d-109">0%</span></span>|<span data-ttu-id="0165d-110">Valor padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.</span><span class="sxs-lookup"><span data-stu-id="0165d-110">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0165d-111">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0165d-111">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0165d-112">1</span><span class="sxs-lookup"><span data-stu-id="0165d-112">-1</span></span>|<span data-ttu-id="0165d-113">Impor componente do Windows e aplicativos de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="0165d-113">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0165d-114">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0165d-114">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0165d-115">2</span><span class="sxs-lookup"><span data-stu-id="0165d-115">-2</span></span>|<span data-ttu-id="0165d-116">Auditar componente do Windows e aplicativos de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="0165d-116">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0165d-117">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0165d-117">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0165d-118">3</span><span class="sxs-lookup"><span data-stu-id="0165d-118">-3</span></span>|<span data-ttu-id="0165d-119">Impor componentes do Windows, aplicativos de armazenamento e bloqueador inteligente.</span><span class="sxs-lookup"><span data-stu-id="0165d-119">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0165d-120">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0165d-120">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0165d-121">4</span><span class="sxs-lookup"><span data-stu-id="0165d-121">-4</span></span>|<span data-ttu-id="0165d-122">Auditar componentes do Windows, aplicativos de armazenamento e bloqueador inteligente.</span><span class="sxs-lookup"><span data-stu-id="0165d-122">Audit Windows components, store apps and smart locker.</span></span>|








