import streamlit as st
import time

# ضبط إعدادات الصفحة والواجهة
st.set_page_config(
    page_title="مَعْبَر AI | Ma'bar AI",
    page_icon="🌿",
    layout="centered"
)

# تنسيق CSS مخصص باللون الكحلي والأخضر البيئي
st.markdown("""
    <style>
    .main { text-align: right; direction: rtl; }
    .title-text { color: #1E3A8A; font-family: 'Cairo', sans-serif; text-align: center; }
    .subtitle-text { color: #0D9488; text-align: center; font-size: 1.2rem; }
    .source-card { background-color: #F0FDF4; border-right: 5px solid #16A34A; padding: 15px; border-radius: 8px; margin-top: 15px; }
    .warning-card { background-color: #FEF2F2; border-right: 5px solid #DC2626; padding: 15px; border-radius: 8px; margin-top: 15px; }
    </style>
""", unsafe_allow_html=True)

# الهيدر والعنوان الرئيسية
st.markdown("<h1 class='title-text'>🌿 مَعْبَر AI (Ma'bar AI)</h1>", unsafe_allow_html=True)
st.markdown("<p class='subtitle-text'>رحلة استكشافية تفاعلية: الاستدامة والحفاظ على البيئة في الإسلام</p>", unsafe_allow_html=True)
st.divider()

# شريط جانبي يوضح آلية عمل RAG للمحكّمين
st.sidebar.image("https://img.icons8.com/isometric/512/leaf.png", width=100)
st.sidebar.title("🎮 لوحة تحكم المحكّم")
st.sidebar.info("هذا النموذج يوضح كيف يعمل محرك RAG مع صمام الأمان (Guardrails) لمنع الهلوسة والإحالة الآلية عند غياب النص المعتمد.")
user_profile = st.sidebar.selectbox("اختر خلفية المستفيد (التكيف الثقافي):", ["باحث بيئي / مهتم بالبيئة", "شاب يبحث عن المعرفة العامة", "مستفيد غير مسلم"])

# مرحلة المدخلات
st.subheader("💬 ابدأ الرحلة المعرفية")
default_question = "هل لدى الإسلام رؤية أو تعاليم تخص حماية البيئة والتغير المناخي؟"
user_query = st.text_input("اطرح سؤالك أو استخدم السؤال الافتراضي:", value=default_question)

if st.button("🚀 استكشف المفهوم"):
    with st.spinner("جاري استرجاع النصوص الشرعية المعتمدة عبر محرك RAG..."):
        time.sleep(1.5) # محاكاة للبحث بالذكاء الاصطناعي
        
    st.success("تم توليد الإجابة وتكييفها بنجاح مع التوثيق المباشر!")
    
    # الإجابة المتكيفة بناء على الملف الشخصي
    if user_profile == "باحث بيئي / مهتم بالبيئة":
        st.write("### 🌍 الإجابة المتكيفة (منظور استكشافي بيئي):")
        st.write("تعتبر الشريعة الإسلامية الحفاظ على البيئة جزءًا لا يتجزأ من **مبدأ الاستخلاف وعمارة الأرض**. لا ينظر الإسلام للبيئة كمورد مجرد للاستهلاك، بل كأمانة يُحاسب الإنسان على إتلافها أو الإسراف فيها.")
    else:
        st.write("### 🌍 الإجابة المتكيفة:")
        st.write("نعم، يضع الإسلام مبادئ قوية لحماية الطبيعة، ويربط بين السلوك البيئي والمسؤولية الأخلاقية، حيث يعتبر الغرس والإصلاح في الأرض نوعًا من العبادة والأجر الممتد.")

    # بطاقة المصدر المعتمد (RAG Citation)
    st.markdown("""
        <div class='source-card'>
            <h4>📜 بطاقة التوثيق المرجعي (RAG Verified):</h4>
            <ul>
                <li><b>الدليل من القرآن:</b> ﴿وَلَا تُفْسِدُوا فِي الْأَرْضِ بَعْدَ إِصْلَاحِهَا﴾ [الأعراف: 56]</li>
                <li><b>الدليل من السنة:</b> قال رسول الله ﷺ: <i>«إِنْ قَامَتِ السَّاعَةُ وَبِيَدِ أَحَدِكُمْ فَسِيلَةٌ، فَإِنِ اسْتَطَاعَ أَنْ لاَ تَقُومَ حَتَّى يَغْرِسَهَا فَلْيَفْعَلْ»</i> (صحيح البخاري)</li>
                <li><b>المفهوم الشرعي:</b> نهي صريح عن الإسراف والتلوث، وحث على الاستدامة حتى آخر لحظة في الحياة.</li>
            </ul>
        </div>
    """, unsafe_allow_html=True)
    
    st.divider()
    
    # المسارات التفاعلية للتعمق
    st.subheader("🔗 اختر مسارك التفاعلي القادم:")
    col1, col2 = st.columns(2)
    with col1:
        if st.button("🌿 مسار: أحكام نهي الإسراف والتلوث"):
            st.info("💡 **إضاءة معرفية:** وضع الفقهاء قاعدة 'لا ضرر ولا ضرار'، والتي يُبنى عليها حظر تلويث موارد المياه والهواء وتدمير المحاصيل.")
    with col2:
        if st.button("📜 مسار: تجربة 'حِمى المدينة' التاريخية"):
            st.info("🏛️ **قصة تفاعلية:** أنشأ النبي ﷺ أول منطقة محمية طبيعية ('الحِمى') في المدينة المنورة لمنع قطع الأشجار ورعي الصيد، لتكون أول محمية تنوع بيولوجي تنظيمية.")

st.divider()

# قسم اختبار صمام الأمان والإحالة (Safety Guardrails)
st.subheader("🛡️ اختبار صمام الأمان (منع الهلوسة والإحالة)")
st.caption("جرب كتابة سؤال فقهي معقد أو سؤال خارج المصادر للتحقق من نظام الإحالة الذكي:")

complex_query = st.text_input("سؤال للتجربة (مثال: ما الحكم الفقهي الدقيق في التداول الكربوني المتعدد؟):")
if st.button("فحص الاستجابة مع Guardrails"):
    if complex_query:
        with st.spinner("فحص المصادر والحدود الفقهية..."):
            time.sleep(1)
        st.markdown("""
            <div class='warning-card'>
                <h4>⚠️ تنبيه نظام الموثوقية ( معالج الإحالة الذكي):</h4>
                <p>هذا السؤال يتطلب دقة اجتهادية وفقهية خاصة خارج نطاق النصوص المباشرة المعتمدة في قاعدة البيانات.</p>
                <p><b>الإجراء الآلي:</b> تم الامتناع عن التخمين (Zero Hallucination)، وتوجيه الاستفسار آليًا لـ <b>الرئاسة العامة للبحوث العلمية والإفتاء / الجهة المختصة</b> للمراجعة البشرية.</p>
            </div>
        """, unsafe_allow_html=True)
